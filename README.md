# Wheel Of Misfortune

## The Game
A role-playing game for incident management training

The Wheel of Misfortune is best done with an on-call group but can be expanded to fit larger groups up to the entire enterprise depending on how thorough and complex you make your scenarios.

My team has found that this works best as a monthly activity, and in general we get through 2 incidents in about an hour as we select an on-call agent using the random picker, spin the wheel (terrifying), work through the incidents – with team leads adding information and hints or extra challenges along the way, then a wrap up of the incident by going through a mock Root Cause Analysis/Blameless Postmortem.

## Hosted
A live demo of this project is available to view at http://wom.twstewart.me/

It is hosted as a static site in an AWS S3 bucket, a walkthrough on setting up a static website using S3 on my personal blog at https://twstewart.me/the-wheel-of-misfortune/


## Testing
One can use the included Dockerfile to test and/or host a local version of the game.

```
$ docker build -t wheel-of-misfortune-test .
$ docker run --name wom-test -d -p 8080:80 wheel-of-misfortune-test
```

# Credits
This project was originally created by https://github.com/dastergon/wheel-of-misfortune 




