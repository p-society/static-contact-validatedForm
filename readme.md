
<p align="center">
<img src="https://user-images.githubusercontent.com/24803604/42569454-28c50a24-852e-11e8-8a7a-fa424515587d.png" />
</p>

## What is its use?

You can add a contact form in your static website like site hosted on Github and able to get response from user.

### Some Cool Features

Sometimes people try to span your email and you get anonymous emails. To avoid this, I have created this so that one has to authenticate their emails before sending message to you.

- Avoid Spam emails
- Can add as many **name** fields in your HTML form.
- Get IP address of the sender

## Preview

![Preview](https://res.cloudinary.com/dsyvg5xwi/image/upload/v1531587414/out3_hpfi8i.gif)

## How to setup your form

1.) fork the repository

2.) Host it on any domain you want, I would suggest [Glitch](https://glitch.com/)

3.) Add an `.env` file in your root folder for reference see [.env.example](https://github.com/knrt10/static-contact-validatedForm/blob/master/.env.example)

4.) Add this to form in your static site

- **Paste your endpoint into your form**

*Change your form's action attribute like this:*

**Important** method should be **GET**

```html
<form method="GET" action="your hosted URL/verify" accept-charset="UTF-8" ></form>
```

- **Add name attribute to every field**

*Inputs, textareas, selects, radios should have unique name attributes*

```html
<input id="name" type="text" name="name" required placeholder="Example:- Messi | Ronaldo">
<input id="email" type="email" name="email" placeholder="Example:- messi@ronaldo.com" required>                
<textarea id="textarea" name="message" placeholder="Enter your message" required ></textarea>
```
**name** field in html form for **email** field is mandatory. Rest you can add as many as you want.

- **All set, you're ready to collect submissions** :fire: Enjoy.

## license

MIT @knrt10
