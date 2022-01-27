# Pythonemail
###send email via python 



import smtplib

server = smtplib.SMTP('smtp.gmail.com', 587)

server.starttls()
server.login('sender@gmail.com', 'password')
server.sendmail('sender@gmail.com', 'receiver@gmail.com', 'message')

print("message sent")
