# Wheel Of Misfortune

## The Game
A role-playing game for incident management training

The Wheel of Misfortune is best done with an on-call group but can be expanded to fit larger groups up to the entire enterprise depending on how thorough and complex you make your scenarios.

My team has found that this works best as a monthly activity, and in general we get through 2 incidents in about an hour as we select an on-call agent using the random picker, spin the wheel (terrifying), work through the incidents – with team leads adding information and hints or extra challenges along the way, then a wrap up of the incident by going through a mock Root Cause Analysis/Blameless Postmortem.

## Hosted
A live demo of this project is available to view at http://wom.twstewart.me/

It is hosted as a static site in an AWS S3 bucket, a walkthrough on setting up a static website using S3 on my personal blog at https://twstewart.me/the-wheel-of-misfortune/


## Testing
One can use the included Dockerfile to test and/or host a local version of the game...or just open the index.html in your favorite browser (low tech testing)

```
$ docker build -t wheel-of-misfortune-test .
$ docker run --name wom-test -d -p 8080:80 wheel-of-misfortune-test
```

## Screenshots
The Wheel of Misfortune Welcome page  
![index.html](screenshots/wom-1.png)

Select an On-call Agent  
Spin the wheel and get started solving incidents  
![incident 10](screenshots/wom-2.png)

# Credits
The concept of a Wheel of Misfortune comes from the Google's [Site Reliability Engineer ebook](https://landing.google.com/sre/sre-book/chapters/accelerating-sre-on-call/#xref_training_disaster-rpg), and the tool was originally created by https://github.com/dastergon/wheel-of-misfortune and then I forked and expanded to fit my team’s needs, added ‘dark mode’ and a random on-call agent selector at https://github.com/twstewart42/wheel-of-misfortune




