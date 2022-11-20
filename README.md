# nikola-ai-and-ml-
nazimraza4321@gmail.com
NIKOLA PROJECT:-


import pyttsx3
import speech_recognition as sr  # in every import file put as pipe.importfile then its downloaded
import datetime
import wikipedia
import webbrowser
import os
import smtpilb

engine = pyttsx3.init('sapi5')
voices = engine.getproperty('voices')
#print(voices[0].id)
//if put 1 then its a lady(sara)
//if put 0 then its a lady(david)
engine.setproperty('voice',voices[0].id)




def speak(audio):
engine.say(audio)
engine.runAndWait()

def wishme();
hour = int(datetime.now().hour)
if hour>=0 and hour<12:
speak("Good Morning!")


elif hour>=12 and hour<18:
speak("Good afternoon!")

else:
speak("Good evening")
speak("I am jarvis sir. Please tell me how may i help you")


def talkcommand();
// it take microphone input from the user and return string output
r = sr.Recognizer()
with sr.Microphone() as source:
print("listening...")
r.pause_threshold = 1
audio = r.listen(source)

//try: (it is used to test whether the programming is working perfect manner or not)
try:
print("recognizing...")
query = r.recognize_google(audio,language='en-in')
print(f"user said: {query}\n")


except Exception as e:
#print(e)
print("say that again please...")
return "None"
 return query


#here put your email and in the down put the reciver
def sendEmail(to, content):
server = smtplib.SMTP('smtp.gmail.com', 587)
server.ehlo()
server.starttls()
server.login('youremailid.gmail.com', 'your-password-here')
server.sendmail('youremail@gmail.com', to, content)
server.close()


if_name_ == "-main_":
#wishMe()
while true:
query = takeCommand().lower()
#logic for executing tasks based on query


// infinite the while lop that is listen only you voice
if 'wikipedia' in query:
speak('searching wikipedia...')
query = query.replace("wikipedia", "")
results = wikipedia.summary(query, sentences=2)
speak("According to wikipedia")
print(results)
speak(results)

elif 'open youtube' in query:
webbrowser.open("youtube.com")

elif 'open google' in query:
webbrowser.open("Google.com")

elif 'open stackoverflow' in query:
webbrowser.open("stackoverflow.com")

elif 'open quora' in query:
webbrowser.open("quora.com")

elif 'open flipkart' in query:
webbrowser.open("flipkart.com")

elif 'open amzon' in query:
webbrowser.open("amzon.com")

elif 'play music' in query:
music_dir = 'D:\\Non Critical\\songs\\favorite songs2'
songs = os.listdir(music_dir)
print(songs)
os.startfile(os.path.join(music_dir, songs)[0]))

elif 'the time' in query:
strTime = datatime.datetime.now().strftime("%H:%M:%s")
speak(f"sir, the time is (strtime)")

elif 'open code' in query:
codepath = "C:\Users\Research-9\Desktop" 
os.strfile(codepath)

elif 'email to harry' in query:
try: 
speak("what should i say?")
content = takeCommand|()
to = "herryjerry047@gmail.com"
sendEmail(to, content)
speak("email has been sent!")
except Exception as e:
print(e)
speak("sorry papa. Iam not able to send this email")
