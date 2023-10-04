# Django_Website_Scraper

mkdir scraper
cd scraper
virutualenv env
pip install django

create project
	django-admin startproject mysite
create app
	django-admin startapp myapp

go to setting.py in mysite folder mention myapp name in installed apps.

pip install requests
pip install beautifulsoup4 

python manage.py shell

>>> import requests
>>> page = requests.get('http://www.google.com')
>>> page

auto reply -> <Response [200]>

page.text

auto reply -> large scripts


from bs4 import BeautifulSoup
>>> soup = BeautifulSoup(page.text,'html.parser')
>>> soup

auto reply -> large scripts


print(soup.prettify())


soup.find_all('a')


>>> for link in soup.find_all('a'):
...     print(link)

exit()


now follow and understand the my github file in the repo
