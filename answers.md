Part 1

#1
let image = document.querySelector('img.profile-image')
image.src = "https://placebear.com/400/400"

#1
let image = document.querySelector('div#left-image img')
image.src = "https://placebear.com/325/325"


#2
let h1 = document.querySelector('h1.highlight')
h1.innerHTML = 'Meke The Bear'

#3
let div = document.querySelector('div#employment h3')
div.innerHTML = '<i class="icon-suitcase"></i> &nbsp; Other Activities'

#4
let body = document.querySelector('body')
body.style.backgroundColor = 'blue'

#5
let body = document.querySelectorAll('.highlight')
body.forEach(element => {
    element.style.color = 'blue'
})

#6
let h1 = document.querySelector('h1')
h1.style.fontFamily = 'monospace'

#7
let a = document.querySelectorAll('a.action-icon-bg')
a.forEach(element => {
    element.style.backgroundColor = 'blue'
})

#8
let input = document.querySelector('input#name')
input.setAttribute('placeholder', 'identify yourself')

#9
let textarea = document.querySelector('textarea#message')
textarea.setAttribute('placeholder', 'state your business')

#10
let input = document.querySelector('input#name')
input.value = 'your nemesis'

#11
let input = document.querySelector('input#email')
input.value = 'koalathebear@gmail.com'

#12
let input = document.querySelector('input#submit')
input.value = 'En garde!'

#13
let input = document.querySelector('input#submit')
input.setAttribute('disabled', 'true')

#14
let span = document.querySelectorAll('span.bio-info-value')
span.forEach(element => {
    element.innerHTML = ' '
})


Part 2

#1
let skill = document.querySelector('div#time-travel').parentNode
skill.parentNode.removeChild(skill)

#1
let Pikachu1 = document.querySelector('div#right-image img').cloneNode()
document.querySelector('div.portfolio-container').appendChild(Pikachu1)


#2
let portfolioContainer = document.querySelector('div.portfolio-container')
let pikachu = document.querySelector('div#right-image img')
for (let i = 0; i < 10; i++) {
    let Pikachu2 = pikachu.cloneNode()
    portfolioContainer.appendChild(Pikachu2)
}

#3
const listItem = document.createElement('li');
listItem.className = 'bio-info-item'
const leftSpan = document.createElement('span');
leftSpan.className = 'bio-info-title'
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);
const rightSpan = document.createElement('span')
rightSpan.className = 'bio-info-value bio-info-last-updated'
const lastUpdatedTime = document.createTextNode(new Date().toLocaleString())
rightSpan.appendChild(lastUpdatedTime)
listItem.appendChild(rightSpan)
document.querySelector('.bio-info').appendChild(listItem)
