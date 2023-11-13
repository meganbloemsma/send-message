# ✨ Send Message spell✨

['Sending'](https://www.dndbeyond.com/spells/sending) is a spell used in Dungeons and Dragons 5e:

>*You send a short message of twenty-five words or less to a creature with which you are familiar. The creature hears the message in its mind, recognizes you as the sender if it knows you, and can answer in a like manner immediately. The spell enables creatures with Intelligence scores of at least 1 to understand the meaning of your message.*

>*You can send the message across any distance and even to other planes of existence, but if the target is on a different plane than you, there is a 5 percent chance that the message doesn't arrive.*

This application works with speech-to-text, using [Cognitive Services Speech SDK](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-sdk).

## How it works

When you run ['send-message.py'](https://github.com/meganbloemsma/send-message/blob/main/src/send-message.py), it will ask you to start speaking. It will record your message real-time and transcribe it to text. If you haven't reached the 25 words yet, it will prompt you to keep going until you have.
Then it will show you what the recipient of the spell will actually have received, capping it at 25 words.

It supports 109 languages or variants. A full list can be found [here](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/language-support?tabs=stt#supported-languages). You will need to adjust the language selected on line 9.

## Setup

The code speaks for itself. Don't forget to set your environment variables before running the code:

    set SPEECH_KEY=your-key
    set SPEECH_REGION=your-region

## Example sentences

Looking for inspiration? Try Critical Role's Jester Lavore and her [Sending spells](https://www.critrolestats.com/jesters-sendings).
Confused? Watch [this](https://www.youtube.com/watch?v=t1G_vFviUVE) (warning: might contain spoilers for Critical Role Campaign 2).
