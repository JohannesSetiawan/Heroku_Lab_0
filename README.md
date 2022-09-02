Tips buat deploy ke Heroku App (https://pbp-fasilkom-ui.github.io/ganjil-2023/assignments/tutorial/tutorial-0):
1. Pastiin App Herokunya ada dan buildpack-nya Python
2. Setelah initialize Django, git init, dan git remote add origin <CLONE_URL>, lebih bagus
   git push origin master dulu. Setelah itu baru deh buat file yg kek Procfile, .gitignore, .github/workflow/dpl.yml di
   github-nya. Atau bisa juga stlh buat tuh file, pull origin master dulu baru add, commit, push.
3. Di secret bakan ada dua variabel, yaitu HEROKU_API_KEY dengan value key API dan HEROKU_APP_NAME dengan value nama app Heroku yang pengen di-link
4. Nama aplikasi_django yang ada di isi Procfile (web: gunicorn aplikasi_django.wsgi --log-file -) itu sama dengan nama proyek django yang udah di-initialize sebelomnya.
