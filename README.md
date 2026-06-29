# She Codes Australia Workshop Tutorials

Welcome to the She Codes Australia One Day Workshop tutorial content! This repository contains all the learning materials for our hands-on coding workshops.

🌐 **Live Site:** [https://tutorials.shecodes.com.au](https://tutorials.shecodes.com.au)

## Workshop Content

Our tutorials cover the following topics:

- **HTML & CSS** - Learn the building blocks of web development
- **JavaScript** - Interactive programming with our Cupcake Smash game
- **Python** - Space Turtle Chomp adventure and programming fundamentals  
- **Django** - Build a dynamic Bakery Finder web application

## Framework and Tools

- **Hugo** v0.147.9 - Static site generator ([Hugo Documentation](https://gohugo.io/))
- **Hugo Relearn Theme** - Documentation theme ([Theme Documentation](https://mcshelby.github.io/hugo-theme-relearn/))
- **Netlify** - Automated deployment and hosting

## Development Setup

### Prerequisites

- Node.js (for package management)
- Hugo (install via npm or download directly)

### Running Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/SheCodesAustralia/new-workshop-content.git
   cd new-workshop-content
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   # Using npm (recommended)
   npx hugo server
   
   # Or if Hugo is installed globally
   hugo server
   ```

4. **View the site**
   Open your browser to [http://localhost:1313](http://localhost:1313)

The site will automatically reload when you make changes to the content.

## Deployment

Deployment is fully automated via Netlify:

- **Production:** Pushes to `main` branch deploy to [https://tutorials.shecodes.com.au](https://tutorials.shecodes.com.au)
- **Preview:** Other branches create preview deployments at `https://[branch-name]--shecodes-tutorials.netlify.app`

## Content Structure

```
content/
├── html_and_css/          # HTML & CSS workshop materials
├── javascript/            # JavaScript Cupcake Smash game tutorial
├── python/               # Python programming workshop
└── django/               # Django web development tutorial
```

## Contributing

1. Create a new branch for your changes
2. Make your edits to the markdown files in the `content/` directory
3. Test locally with `hugo server`
4. Push your branch to see a preview deployment
5. Create a pull request when ready

## Content Guidelines

- All tutorial content is written in Markdown
- Images should be placed in the appropriate `images/` folder within each section
- Use the Hugo shortcodes provided by the Relearn theme for enhanced formatting
- Test certificate generation functionality when editing certificate pages

## Support

For questions about the workshop content or technical issues, please create an issue in this repository or contact the She Codes Australia team.

---

**She Codes Australia** - Empowering women in technology through education and community.

---

# TODO

> [!CAUTION]  
> Remember to delete this section once the changes are complete.

**Legend:** 
- **Install** = Python install step
- **Invoke** = Python run from the terminal
- **Venv** = virtual environment creation 
- **pip** / **django-admin** = related terminal commands
- **Screenshot** = image that may need updating.

### [content/python/getting_started/_index.md](content/python/getting_started/_index.md)

- [x] **Install** — "We need Python before we can start... start by installing Python" (intro).
- [x] **Invoke** — macOS/Linux version check: `python3 --version`.
- [x] **Invoke** — Windows version check: `py --version`.
- [x] **Install** — macOS: change Security & Privacy settings before installing.
- [x] **Install** — macOS: download the installer from https://www.python.org/downloads/ and run the `.pkg`.
- [x] **Invoke** — Linux version check: `python3 --version`.
- [x] **Install** — Linux (Debian/Ubuntu): `sudo apt-get install python3`.
- [x] **Install** — Linux (Fedora up to 21): `sudo yum install python3`.
- [x] **Install** — Linux (Fedora 22+): `sudo dnf install python3`.
- [x] **Install** — Linux (openSUSE): `sudo zypper install python3`.
- [x] **Invoke** — Verify install: `python3 --version`.
- [x] **Install** — Windows: download from https://www.python.org/downloads/windows/ and run the executable installer (tick "Add Python 3.x to PATH").
- [x] **Install** — Windows: install Python from the Microsoft Store.
- [x] **Screenshot** — Windows Run dialog (`cmd`): [windows-plus-r.png](content/python/getting_started/python_installation/images/windows-plus-r.png).
- [x] **Screenshot** — Windows "Add Python to PATH" installer screen: [add_python_to_windows_path.png](content/python/getting_started/python_installation/images/add_python_to_windows_path.png).

### [content/python/getting_started/how_to_python/_index.md](content/python/getting_started/how_to_python/_index.md)

- [x] **Invoke** — Open the Python REPL: type `python` (Windows) or `python3` (Mac/Linux).
- [x] **Invoke** — Launching the Python console: `python3`.
- [x] **Invoke** — Run a script: `python3 python_intro.py`.
- [x] **Invoke** — Windows run a script: `python python_intro.py`.
- [x] **Invoke** — Re-running `python3 python_intro.py` (repeated throughout the exercises).

### [content/Django/getting_started/_index.md](content/Django/getting_started/_index.md)

- [ ] **Install** — "Install Python" section intro.
- [ ] **Install** — macOS: download the Python 3.x installer from python.org and run it.
- [ ] **Install** — Windows: download Python from python.org (tick "Add Python 3 to PATH").
- [ ] **Invoke** — Linux version check: `python3 --version`.
- [ ] **Install** — Linux: `sudo apt install python3` / `sudo dnf install python3` / `sudo zypper install python3`.
- [ ] **Venv** — "Set up virtual environment and install Django" section intro.
- [ ] **Venv** — macOS/Linux: `python3 -m venv myvenv`.
- [ ] **Venv** — Windows: `python -m venv myvenv`.
- [ ] **pip** — `pip install --upgrade pip`.
- [ ] **pip** — `pip install -r requirements.txt`.

### [content/Django/your_first_django_project/_index.md](content/Django/your_first_django_project/_index.md)

- [ ] **django-admin** — macOS/Linux: `django-admin startproject bakery_project .`.
- [ ] **django-admin** — Windows: `django-admin.exe startproject bakery_project .`.
- [ ] **Invoke** — `python manage.py runserver`.
- [ ] **Invoke** — Windows `UnicodeDecodeError` fix: `python manage.py runserver 0:8000`.

### [content/Django/lets_get_appy/_index.md](content/Django/lets_get_appy/_index.md)

- [ ] **Invoke** — `python manage.py startapp bakeries`.
- [ ] **Invoke** — Windows: `python manage.py startapp bakeries`.
- [ ] **Invoke** — `python manage.py runserver`.
- [ ] **Invoke** — `python3 manage.py runserver`.

### [content/Django/shes_a_model/_index.md](content/Django/shes_a_model/_index.md)

- [ ] **Invoke** — `python manage.py migrate`.
- [ ] **Invoke** — `python manage.py makemigrations bakeries`.
- [ ] **Invoke** — `python manage.py migrate bakeries`.

### [content/Django/django_admin/_index.md](content/Django/django_admin/_index.md)

- [ ] **Invoke** — `python manage.py runserver`.
- [ ] **Invoke** — `python3 manage.py runserver`.
- [ ] **Invoke** — `python manage.py createsuperuser`.
- [ ] **Invoke** — `python3 manage.py createsuperuser`.
- [ ] **Invoke** — `python manage.py createsuperuser`.

## Notes

- The `content/python/` tutorial does not create or use a virtual environment.
- [python-installation-options.png](content/python/getting_started/python_installation/images/python-installation-options.png) is a Python installer options screenshot that is not referenced by any markdown file (possibly orphaned — worth confirming).

---

# Changelog

> [!CAUTION]  
> Remember to include the following in the PR and then delete from this README.

## [Getting Started](./content/python/getting_started/_index.md)

- Removed a section in Mac instructions on checking whether Python is already installed. Irrelevant because we'll be using UV.
- Removed a section in Mac instructions that told the user to make sure their Mac was configured to allow non-Apple Store installs. Unnecessary because UV is amazing.
- Modified Mac install instructions to use UV
- Cut down the various flavours of Linux install instructions to a single blanket UV installation
- Modified Windows install instructions to use UV

## [How To Python](content/python/getting_started/how_to_python/_index.md)
- Swapped invocation method to `uv run ...` throughout
- Removed dimorphic instructions for different operating systems
- Bugfix: capitalisation:

   ````diff
   Nice, huh? To see your name in uppercase letters, try typing:

   <!-- {% filename %}command-line{% filename %} -->
   ```python {title="python"}
   >>> "Kate".upper()
   - 'Kate'
   + 'KATE'
   ```
   ````