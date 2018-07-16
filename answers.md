1) Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.

var profilePic = document.querySelector("img.profile-image")

2)Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

var profilePic = document.querySelector("img.profile-image").src="https://imageshack.com/i/polCSCzvp";


3)Select the heading that says "Panda the Bear" and change it to your own name.

var title = document.querySelector("h1.highlight").innerText ="Haggai Lerman"

4)Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

var employment = document.querySelectorAll("h3.info-title");
employment[1]["innerText"] = "Job Experience"


5)Change the colour of the body.

bodyColour = document.querySelector('body').style.background = 'blue'
"blue"

6)Change the colour of each element using the highlight class. Use a for loop to do this.

colourElement = document.querySelectorAll('.highlight').forEach(function(element){element.style.color = "yellow";});


7)Change the font family of the h1 to 'monospace'.

h1FontType = document.querySelector("h1").style.fontFamily = 'monospace'


8)Find a way to select the round icons in the sidebar and then change their colour.

h1FontType = document.querySelectorAll('.action-icon-bg').forEach(function(element){
    element.style.backgroundColor = 'blue'
    });

9)Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

namePlaceHolder = document.querySelector('form input[placeholder]')
namePlaceHolder["placeholder"] = " dentify yourself"

10)Change the placeholder attribute of the message field to "state your business".

messagePaceholder = document.querySelector('#message')["placeholder"] ='state your business';
"state your business"

11)Give the name field a "value" attribute of "your nemesis".

namePlaceHolder = document.querySelector('form input[placeholder]')['name'] = 'your nemesis';

12)Change the value attribute of the email field to "koalathebear@gmail.com".

emailField = document.querySelector('#email')['placeholder'] = "koalathebear@gmail.com";



13) Change the value of the submit button on the contact form to "En garde!".
    submitForm = document.getElementById('submit'); submitForm.value = 'En garde!';


14)We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

submitForm.disabled = true;


15)We should help Panda protect their privacy by erasing their personal details from the sidebar.

personalInfo = document.querySelector(".bio-info");
personalInfo.remove();
