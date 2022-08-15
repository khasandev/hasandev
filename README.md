# hasandev
use strict'
JS
document.addEventListener('DOMContentLoaded', () => {
    const adv = document.querySelectorAll('.promo__adv img '),
    wrapper = document.querySelector('.promo__bg'),
    genre = wrapper.querySelector('.promo__genre'),
    serialList = document.querySelector('.promo__interactive-list'),
    addForm = document.querySelector('form.add'),
    inputVal = addForm.querySelector('.adding__input'),
    checkbox = addForm.querySelector("[type = 'checkbox']")




    const seriesDB = {
        series: [
            'OMAR',
            'THE FINAL LEGACY',
            'ERTUGRUL',
        ' MAGNIFICENT CENTURY',
            'GREAT SELJUKS: GUARDIANS...',
        ],
    }

    addForm.addEventListener('submit', (event) => {
        event.preventDefault()

        const newSeries = inputVal.value  // bu input qiymatini olib beradi
        const checkbox = checkbox.checked // checked bo'lgandagi qiymatini oladi
    })

    adv.forEach((item) => {
        item.remove()
    })


    genre.textContent = 'Comedy'

    wrapper.style.backgroundImage = 'url("content2_files/1.jpg")'


    serialList.innerHTML = ''


    seriesDB.series.forEach((item, idx) => {
        serialList.innerHTML += `
        <li class="promo__interactive-item">${idx + 1}  ${item}
        OMAR
        <div class="delete"></div>
        </li>
    `
})
})












<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Series DB</title>
    <link
      href="https://fonts.googleapis.com/css?family=Roboto:300,400,700&display=swap&subset=cyrillic-ext"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <main class="promo">
      <div class="promo__content">
        <div class="promo__bg">
          <div class="promo__genre">DRAMA</div>
          <div class="promo__title">BEST EARTH</div>
          <div class="promo__descr">
            THE STORY OF A MAN WHO SURVIVED ON AN ALIEN PLANET ALONE
          </div>
          <div class="promo__ratings">
            <span>IMDb: 8.0</span>
            <span>Movie star: 7.7</span>
          </div>
        </div>
        <div class="promo__interactive">
          <div>
            <div class="promo__interactive-title">RECENT SERIES</div>
            <ul class="promo__interactive-list">
              <li class="promo__interactive-item">
                OMAR
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                The Final Legacy
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                ERTUGRUL
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                MAGNIFICENT CENTURY
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                GREAT SELJUKS: GUARDIANS...
                <div class="delete"></div>
              </li>
            </ul>
          </div>
          <div>
            <form class="add">
              <div class="promo__interactive-title">ADD NEW SERIES</div>
              <span>Name of series</span>
              <input
                class="adding__input"
                type="text"
                placeholder="What has already been viewed...?"
              />
              <span>Make it your favorite?</span>
              <input type="checkbox" />
              <span class="yes">Yes!</span>
              <button>Submit</button>
            </form>
          </div>
        </div>
      </div>
      <div class="promo__adv">
        <div class="promo__adv-title">Advertising from sponsors</div>
        <img src="facebook_files/facebook.jpg" alt="some picture" />
        <img src="media_files/media.png" alt="some picture" />
        <img src="content2_files/content_2.jpg" alt="some picture" />
        <img src="content3_files/content_3.png" alt="some picture" />
      </div>
    </main>

    <script src="script.js"></script>
  </body>
</html>











<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Series DB</title>
    <link
      href="https://fonts.googleapis.com/css?family=Roboto:300,400,700&display=swap&subset=cyrillic-ext"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <main class="promo">
      <div class="promo__content">
        <div class="promo__bg">
          <div class="promo__genre">DRAMA</div>
          <div class="promo__title">BEST EARTH</div>
          <div class="promo__descr">
            THE STORY OF A MAN WHO SURVIVED ON AN ALIEN PLANET ALONE
          </div>
          <div class="promo__ratings">
            <span>IMDb: 8.0</span>
            <span>Movie star: 7.7</span>
          </div>
        </div>
        <div class="promo__interactive">
          <div>
            <div class="promo__interactive-title">RECENT SERIES</div>
            <ul class="promo__interactive-list">
              <li class="promo__interactive-item">
                OMAR
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                The Final Legacy
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                ERTUGRUL
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                MAGNIFICENT CENTURY
                <div class="delete"></div>
              </li>
              <li class="promo__interactive-item">
                GREAT SELJUKS: GUARDIANS...
                <div class="delete"></div>
              </li>
            </ul>
          </div>
          <div>
            <form class="add">
              <div class="promo__interactive-title">ADD NEW SERIES</div>
              <span>Name of series</span>
              <input
                class="adding__input"
                type="text"
                placeholder="What has already been viewed...?"
              />
              <span>Make it your favorite?</span>
              <input type="checkbox" />
              <span class="yes">Yes!</span>
              <button>Submit</button>
            </form>
          </div>
        </div>
      </div>
      <div class="promo__adv">
        <div class="promo__adv-title">Advertising from sponsors</div>
        <img src="facebook_files/facebook.jpg" alt="some picture" />
        <img src="media_files/media.png" alt="some picture" />
        <img src="content2_files/content_2.jpg" alt="some picture" />
        <img src="content3_files/content_3.png" alt="some picture" />
      </div>
    </main>

    <script src="script.js"></script>
  </body>
</html>
