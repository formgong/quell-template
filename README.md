# Quell: an architect and engineer portfolio site with a Formgong form

**Live demo:** https://quell.formgong.com · Download: the [latest release](https://github.com/formgong/quell-template/releases/latest) zip.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/formgong/quell-template) [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fformgong%2Fquell-template&project-name=quell&repository-name=quell)

Each button copies the site to your GitHub and publishes it. Then replace `fk_your_access_key` in `index.html` of your copy with your Formgong access key (free at https://formgong.com/new) and commit: the host republishes on its own.

Сайт-портфоліо архітектора чи інженера з формою Формгонг

A one-page portfolio for an architect, a structural engineer or a small design studio, in a single `index.html` plus an `img/` folder. The demo studio, Mara Quell, its buildings, quotes and contacts are fictional.

- **Hero.** A full-screen photo with the name split in two giant words, top left and bottom right, and a menu line across the middle. As you scroll, the two words slide apart, the menu rises and the photo stays in place.
- **Intro.** A dark panel rises over the photo with a large statement, then three tall photos with captions.
- **Work timeline.** A thin line runs down the middle and fills as you scroll, with a dot at its end. Eight projects sit on both sides of it at different sizes, each with its year on the line. On hover the other photos dim and the project's name and structure appear beside it. On phones the projects stack, with the name always shown.
- **Practice.** The studio's place and years, a large paragraph, a wide photo and a short bio.
- **Statement and quote.** A large two-line heading and a quote.
- **Start a project.** A Formgong form with name, email, a choice of project type, place, timing and a message.
- **Footer.** A closing line, the credits and the studio name across the full width, filled with a photo.

Text reveals line by line, headings word by word, and photos come into focus as they scroll in. With `prefers-reduced-motion: reduce` all of it is switched off and the page stays still.

## English

**Set up the form**

1. Create a form in the Formgong dashboard and copy its access key.
2. In `index.html`, replace `fk_your_access_key` with that key.
3. The form sends `name`, `email`, `project`, `location`, `timing`, `message` and a hidden `subject`. It shows thanks only when Formgong answers `success: true`. If the answer is anything else, it shows the error and keeps what was typed.

**Edit**

- Colours are at the top of the styles: `--bg` for the page, `--ink` for text, `--line` for the thin rules and `--accent` for focus rings.
- The name is two words in the hero (`.w1` and `.w2`) and once more in the footer (`.giant`). The footer name is sized by the script to fill the width exactly.
- Each project in the timeline is an `<article class="item">`. Its `--c` sets the columns it takes on a 12-column grid, such as `--c: 4 / span 3`. Add the class `l` to projects on the right half, so their name appears on the left.
- Replace the photos in `img/`, keeping the file names, or change the paths in `index.html`.

**Images.** The fifteen photos were generated for this template with ChatGPT image generation (OpenAI) and saved as WebP, about 1.4 MB in all. The buildings and the person in them are fictional. You may use them in your own site, but replace them with your own work before launch.

The "Powered by Formgong" links point to `https://formgong.com/review-page/fk_your_access_key`, so the same find and replace covers them. Once your key is in, the first click from your published site makes your own public review page on Formgong, where clients read and leave reviews, and every later click opens it. Switch the page off in Formgong (Reviews → your site → Settings) or change those links.

## Українська

Односторінковий сайт-портфоліо для архітектора, інженера-конструктора чи невеликої студії. Студія Mara Quell, її будівлі, цитати й контакти вигадані.

На сторінці:

- перший екран із фото на весь екран, де ім'я розділене на два великі слова: під час прокрутки вони роз'їжджаються, а меню піднімається;
- темна панель із заявою, що наїжджає на фото, і три високі фото;
- таймлайн робіт: лінія посередині заповнюється під час прокрутки, вісім проєктів стоять по обидва боки, а під курсором з'являються назва й конструкція;
- блок про студію, великий заголовок і цитата;
- форма «Start a project» з вибором типу проєкту;
- футер, де ім'я студії на всю ширину заповнене фото.

**Налаштування.** Створіть форму в кабінеті Formgong і замініть `fk_your_access_key` у `index.html` на свій ключ. Подяка з'являється лише тоді, коли Formgong відповідає `success: true`.

**Зображення:** п'ятнадцять фото згенеровано для цього шаблону в ChatGPT (OpenAI) і збережено у WebP, разом близько 1,4 МБ. Будівлі й людина на них вигадані. Їх можна використовувати, але перед запуском замініть їх своїми роботами.

MIT license.

Посилання «Powered by Formgong» ведуть на `https://formgong.com/review-page/fk_your_access_key`, тож та сама заміна ключа оновить і їх. Коли ключ стоїть, перший перехід з вашого опублікованого сайту створює вашу публічну сторінку відгуків на Formgong, де клієнти читають і залишають відгуки; далі посилання відкриває її. Вимкнути сторінку можна у Formgong (Відгуки → ваш сайт → Налаштування) або змінити ці посилання.
