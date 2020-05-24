Various things that I did not want on the website itself.

## Feedburner
http://feeds.feedburner.com/Philozophy

## Fonts
https://www.onlinewebfonts.com/search?q=Caslon

- public health and liberty:
  - specific examples: church closures, lockdowns for covid 19
  - show why we won't find rational grounds to decide that question:
    - probabilities, future, subjective risk affinity
- fallacies
- stories

Can we have answers to all our questions, or do we have limitations?

I liked the first part - but I think you posted it into the wrong track
The second-to-last paragraph feels like you're trying to say, "Be an atheist" without using the word 'religion' - though maybe now I'm being presumptive because of our previous conversations!
Which is a personal opinion, not really a discussion of a philosophical idea
Though I guess it is Epistemology...
The spirit of the post reminded me of Protagoras, the Sophist
"You can't know for sure whether your stories are correct or not, so you shouldn't enforce them on others."
The part un-said is, "That's the job of the state!"
Today at 12:32 PM
ah yes - it's not the right track
you might be correct about the second to last paragraph, but I think it's broader - but you might not be incorrect
and you are saying I'm a sophist! now that's bad
the job of the state?
I think the second to last is still philosophy, in that I am proposing a way of being in the world
I am partly proposing an answer to the perennial question of "how we should conduct our lives"
of course, any solution uttered by one person is going to be their opinion
unless there is an absolute, universal solution
which at present is not really forthcoming
the second to last is highly philosophical, though yes, it presents one position - one could argue that it is ok to lead your life on made up stories. One could argue that some stories have more merits than others (science has proven to work much better for medicine than religion). One could argue that we are story creatures, and that stories are a political currency. One could argue that some stories hurt us, while some help us. All things I do intend to explore in further posts.

[19:53, 5/18/2020] Frank: le seul domaine ou on essaie d'enlever l'opinon, c'est la science
[19:53, 5/18/2020] Frank: c'est d'ailleurs la caracteristique fondamentale de l'histoire qu'elabore la science

I'm getting more pushback that my second to last paragraph is opinion
I think it ruffles quite a few feathers
and also, that philosophy has a fair bit of opinion in it in general
the only place where we really weed out opinion is in science
where we replace opinion by verification against Nature
otherwise, there is little objectivity out there
if you notice, Plato purports to have a method when examining various questions, which would be better than mere opinion, but I'm not sure the conclusions of the dialogues are always "objective" - when they even have a conclusion
if we always require objectivity from philosophy, it's going to be quite limited - and in fact, we are going to do science, and not philosophy, I'm afraid


The software you can use is Vosk-api, a modern speech recognition toolkit based on neural networks. It supports 7+ languages and works on variety of platforms including RPi and mobile.

First you convert the file to the required format and then you recognize it:

ffmpeg -i file.mp3 -ar 16000 -ac 1 file.wav
Then install vosk-api with pip:

pip3 install vosk
Then use these steps:

git clone https://github.com/alphacep/vosk-api
cd vosk-api/python/example
wget https://github.com/alphacep/kaldi-android-demo/releases/download/2020-01/alphacep-model-android-en-us-0.3.tar.gz
tar xf alphacep-model-android-en-us-0.3.tar.gz 
mv alphacep-model-android-en-us-0.3 model-en
python3 ./test_simple.py file.wav > file.json

