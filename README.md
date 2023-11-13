# ✨ Send Message ✨

['Sending'](https://www.dndbeyond.com/spells/sending) is a spell used in Dungeons and Dragons 5e:

>*You send a short message of twenty-five words or less to a creature with which you are familiar. The creature hears the message in its mind, recognizes you as the sender if it knows you, and can answer in a like manner immediately. The spell enables creatures with Intelligence scores of at least 1 to understand the meaning of your message.*

>*You can send the message across any distance and even to other planes of existence, but if the target is on a different plane than you, there is a 5 percent chance that the message doesn't arrive.*

This application works with voice-to-text, using [OpenAI's 'Whisper](https://github.com/davabase/whisper_real_time/blob/master/transcribe_demo.py), and counts the words for you. If you reach the maximum (25 words) it will give you a notification.

It is also applicable to other spells, such as 'Magic Mouth'.

## Notes

Online there are multiple speech recognition or voice-to-text services available. A quick browse on huggingface.io comes up with [over 10.000 models](https://huggingface.co/models?pipeline_tag=automatic-speech-recognition&sort=trending).

After spending an entire morning trying to set up whisper and failing **I am going the easy route: using cognitive services [Speech SDK](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-sdk).**