# Build an Alexa How-To Skill in ASK Python SDK
<img src="https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/quiz-game/header._TTH_.png" />

[![Voice User Interface](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/1-locked._TTH_.png)](./1-voice-user-interface.md)[![Lambda Function](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/2-locked._TTH_.png)](./2-lambda-function.md)[![Connect VUI to Code](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/3-locked._TTH_.png)](./3-connect-vui-to-code.md)[![Testing](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/4-locked._TTH_.png)](./4-testing.md)[![Next Steps](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/5-on._TTH_.png)](./5-next-steps.md)

## Customize the Skill to be Yours

At this point, you should have a working copy of our How To skill.  In order to make it your own, you will need to customize it with data and responses that you create. The data and responses can be found in the [data.py](../lambda/alexa/py/data.py) file. Here are the things you will need to change:

1.  **New data.** You will need to provide a set of data for your topic.  We recommend a minimum of 25, but a total closer to 100 offers a better experience.

    1.  **Open a copy of data.py.** If you haven't already downloaded the code for this project, [you can find a copy of data.py here](../lambda/py/alexa/data.py).  You can use a simple, lightweight code editor like [Atom](http://atom.io), [Sublime Text](http://sublimetext.com), or [VSCode](http://code.visualstudio.com).

    2.  **Look at the RECIPES_EN_US**  This is the list of minecraft recipes in your skill. Add more recipes into the mapping.

    3.  **When you have replaced the data in `data.py`, you need to upload the latest data into Lambda.**  Copy the updated contents into the ``skill_env`` folder, zip the contents of the ``skill_env`` folder and upload it to AWS Lambda as discussed in the "**Finish configuring your function**" step in [Lambda setup documentation](./2-lambda-function.md). Test your skill through the Alexa Simulator on the developer portal, with the updated changes.

2.  **New sentences to respond to your users.** There are several sentences and responses that you will want to customize for your skill.

    1.  **Go back to your copy of [lambda_function.py](../lambda/lambda_function.py).**

    2.  **Look for lines like this: "WELCOME_MESSAGE = _("Welcome..""** These are strings that hold phrases for Alexa to respond with.  Customize them to make it as varied and conversational as time allows.

    3.  **Continue through ``data.py`` until you reach the bottom of the file.**  This will ensure that you cover each of the Alexa responses that you need to update.

3.  **New language.** If you are creating this skill for another language other than English, you will need to make sure Alexa's responses are also in that language. The process of generating locale specific translations can be checked in the [localization guide](./localization.md).

    *  For example, if you are creating your skill in German, every single response that Alexa makes has to be in German.  You can't use English responses or your skill will fail certification.
    *  For sample usage, we provided the translated files for ``us_GB`` and ``de_DE`` locales. They can be checked in the [locales folder](../lambda/py/locales).
    
4.  **Updated code.** Once you have made the updates, you need to upload the latest data into Lambda.**  Copy the updated contents into the ``skill_env`` folder, zip the contents of the ``skill_env`` folder and upload it to AWS Lambda as discussed in the "**Finish configuring your function**" step in [Lambda setup documentation](./2-lambda-function.md). Test your skill through the Alexa Simulator on the developer portal, with the updated changes.

5. 6.  **Once you have made the updates listed on this page, you can click "Launch" in the top navigation to move on to Publishing and Certification of your skill.**

    <!--![Dev Portal Next](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/general/3-7-next-button._TTH_.png) -->


[![Next](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/general/buttons/button_next_publication._TTH_.png)](6-publication.md)
    
   
