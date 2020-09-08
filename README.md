# Pee Pee
Flask web app examining user's health with his/her pee color 💦

![image](https://user-images.githubusercontent.com/42399232/92462120-00c6ac80-f205-11ea-8cd8-d41ed93a2c9c.png)

## Reason I developed
In the cloud server study I was in, I've got an idea of developing AI pee examiner web-app from the professor. I thought the idea was hillarious and it might be a small fun project, and also I wanted to try building Flask app on Cloud Server.(NHN TOAST) Built this project in 2 weeks with one team member. The color distribution criteria is little awkward, but uploading file and examining the dominated color in the picture works pretty well.

## Algorithm
1. Crop the center of the image user uploaded by 100x100px size.
2. KMeans extract the dominated color from the section.
3. Find a criteria which the color is in. (Referenced [Check my health with 11 different color of pee](https://news.joins.com/article/21381482))
4. Print the result.

## Built With
- Python
  - CV2(4.2.0.32)
  - KMeans
  - Flask
- Docker ([docker image](https://github.com/tiangolo/uwsgi-nginx-flask-docker))
  - uwsgi
  - Nginx
  - Flask
- AWS
