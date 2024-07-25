## Get Data By Parameters

By tag
```
# get all <h1> elements
# on the page
h1_elements = soup.find_all('h1')
```

By id

```
# get the element with id="main-title"
main_title_element = soup.find(id='main-title')
```

By text
```
# find the footer element
# based on the text it contains
footer_element = soup.find(text={'Powered by Me'})
```

By attribute
```
# find the email input element
# through its "name" attribute
email_element = soup.find(attrs={'name': 'email'})
```

By class
```
# find all the centered elements
# on the page
centered_element = soup.find_all(class_='text-center')
```

### Concatenating Parameters

```
# get all "li" elements
# in the ".navbar" element
soup.find(class_='navbar').find_all('li')
```

```
# get all "li" elements
# in the ".navbar" element
soup.select('.navbar > li')
```