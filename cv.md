# My CV

## Nikita Mishchenko
![My picture]("C:\Users\GamerOne\Pictures\me\IMG_3270.jpg")

## About me

I am a *hardworking* student, who is always ready to stay after classes and complete an extra task. For the last few years I didn't even have proper holidays due to me being and olympiad participant in English Language. While my classmates were relaxing on their holidays and being couch potatoes, I was attending school in the morning and stayed there for *4 hours*.

## My skills

* My time management is great.
    + Even though I always have a lot work to do, I have planned all of it out perfectly, so I manage to do everything and still get the right amount of rest, which is necessary, since otherwise my productivity will drop drastically
* My leadership skills are on a high level.
    + I am capable of being a good leader. I have done many courses in this sphere. When we get a task to be done in teams in school, I always tend to be the leader of the group.
* My code knowledge is exceptional.
    + I have been studying code for over *2 years* now and I'm not planning to stop. I know **HTML**, **CSS**, **JavaScript** and I am targeting to learn **Node.js** and **React** in the near future

## Here is an example of my code:

```
start.addEventListener('click', startGame)

function startGame(){
    score = 0
    isGameActive = true
    start.classList.add('hide')
    game.style.backgroundColor = 'white'
    timeh1.classList.remove('hide')
    resulth1.classList.add('hide')
    time.innerText = inputTime.value
    inputTime.setAttribute('disabled', 'disabled')

    let interval = setInterval(() => {
        let currentTime = +time.innerText
        if (currentTime <= 0) {
            clearInterval(interval);
            endGame()
        }
        else {
            currentTime = currentTime - 0.1
            time.innerText = currentTime.toFixed(1)
        }
     }, 100);

    renderBox()
}

function renderBox(){
    if (!isGameActive) {
        return;
        }
    game.innerHTML='';
    let randomSize = getRandom(30, 100)
    let maxDelta = 300 - randomSize
    let div = document.createElement('div')
    div.style.width = randomSize+'px';
    div.style.height = randomSize+'px';
    div.style.position = 'absolute'
    div.style.backgroundColor = 'black'
    div.style.top = getRandom(0, maxDelta)+'px'
    div.style.left = getRandom(0, maxDelta)+'px'
    div.style.cursor = 'pointer'
    div.classList.add('box')
    game.appendChild(div)
}


game.addEventListener('click', gameBoxClick)

function gameBoxClick(event){
    if (event.target.classList.contains('box')) {
        score++;
        renderBox()
    }    
}

function getRandom(min, max) {
    return (Math.floor(Math.random() * (max - min) + min)) 
  }

function endGame(){
    isGameActive = false;
    game.innerHTML='';
    start.classList.remove('hide')
    game.style.backgroundColor = '#CCCCCC'
    timeh1.classList.add('hide')
    resulth1.classList.remove('hide')
    inputTime.removeAttribute('disabled');
    result.innerText = score
}

inputTime.addEventListener('change', (event) => {
    time.innerText = inputTime.value
    timeh1.classList.remove('hide')
    resulth1.classList.add('hide')
})
```

## And here is the result:
![result-1](C:\Users\GamerOne\Downloads\Screenshot 2022-11-13 172444.png)
![result-2](C:\Users\GamerOne\Downloads\Screenshot 2022-11-13 172526.png)

## My work experience

I have done countless tasks that require strong notion of html, css and js. The code above is one of the examples. Also I have completed two big projects, in which me and my team would create a fully-functional website. The first one is about identification of birds, and the other one is an internet museum, where you can explore famous paintings online.

## My education

So far, I'm studying in the 10th grade. This is my third year of coding. Just like I've mentioned before, I have done a lot of courses and listened to a staggering amount of lectures on different topics, in particular leadership, applying for a job, teamwork, studying abroad etc. Moreover, half of these courses were in English, which definetely boosted my knowledge of the language.

## Speaking of English...

My level of English is stunningly high, I've been studying it for my whole life. I go to a gymnasia with an English profile and I am the best at English among my parallel. In addition to that, previous year I participated in a 10th form olimpiad, even though I was in the 9th grade at that time. As a result, I won a 3rd degree diploma on the city olimpiad. I am able to speak English fluently and have no problem with communicating with foreigners.