// Changing Profile Picture
var profilePicture = document.querySelector('.profile-image')
profilePicture.src = 'https://picsum.photos/id/1071/400/400'

// Changing Portfolio Picture
var photo = document.querySelector('div #left-image.portfolio-image')
photo.src = 'https://picsum.photos/id/831/325/325'

// Changing the page title
var headtitle = document.querySelector('h1.highlight')
headtitle.innerHTML = "Dave's Page"

Changing more titles that are nested down there

var education = document.querySelector('div#education.info-inner-container h3.info-title')
education.innerHTML = '<i class="icon-book"></i> &nbsp; Dave\'s Poop'
// changed the HTML beacuse there was no label on the text, tried both methods of innerText and innerHTML

//changing body background colour
body = document.querySelector('body')
body.style.background ="red"

// also tried the bottom which worked:
$(body).css('background','red')

// Change the colour of each element using the highlight class. Use a for loop to do this.
var highlight = document.querySelectorAll('.highlight')
for ( var i = 0; i < highlight.length; i++) { highlight[i].style.background = "red" }

// Change the font family of the h1 to 'monospace'.
var h1 = document.querySelectorAll('h1')
for ( var i = 0; i < h1.length; i++) { h1[i].style.fontFamily = "monospace" }

// Find a way to select the round icons in the sidebar and then change their colour.
var iconBack = document.querySelectorAll('a.action-icon-bg')
for ( var i = 0; i < iconBack.length; i++) { iconBack[i].style.backgroundColor = "blue" }


// Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

var nameForm = document.querySelector('input#name.contact-info')
nameForm.placeholder = "identify yourself"

// Change the placeholder attribute of the message field to "state your business".
var messageArea = document.querySelector('textarea#message')
messageArea.placeholder = "state your business"

// Give the name field a "value" attribute of "your nemesis".
nameForm.value = "your nemesis"

// Change the value attribute of the email field to "koalathebear@gmail.com".
var email = document.querySelector('input#email.contact-info')
email.value = "koalathebear@gmail.com"

// Change the value of the submit button on the contact form to "En garde!".
var formSubmit = document.querySelector('input#submit')
formSubmit.value = "engarde"


// We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).
$("input#submit").prop('disabled', true);



// We should help Panda protect their privacy by erasing their personal details from the sidebar.
