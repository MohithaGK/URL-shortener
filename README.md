# URL-shortener
Have you ever thought about or tried to shorten the length of the URL? Then, there are plenty of libraries that is available in python programming language to help us do the task.

import pyshorteners # package installation
link = input("enter the link: ")# https://github.com/MohithaGK
shorte = pyshorteners.Shortener()#calling the Class

x = shorte.tinyurl.short(link)
y = shorte.isgd.short(link)
z = shorte.osdb.short(link)
print("The tinyurl link :" + x)
print(y)
print(z)

# url shortner using bitly
Access_Token = "3e1a2cd3a5fffc994978e4b32b20db1c48a5c7f7" #token was been created using bitly account
short_url = pyshorteners.Shortener(api_key = Access_Token)
a = short_url.bitly.short(link)
print("the bitly link is : "+ a)
