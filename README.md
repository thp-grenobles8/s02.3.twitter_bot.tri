0) Git init et push sur Github

git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/thp-grenobles8/s02.3.twitter_bot.tri.git
git push -u origin master


1) Pour initialiser la gem rspec pour les tests, va créer le dossier spec :
		$ rspec --init

2)  Pour créer le Gemfile.lock :
		$ bundle install

3)  Pour tester l'écriture de ton code (à taper dans le dossier avec fichier .rb) :
		$ rubocop

4) 	Pour utiliser le débugger PRY :
		require 'pry' en haut de ton programme concerné, puis binding.pry pour exécuter PRY dans ton code.

5)  POUR CACHER SES CLEFS API :
		require 'dotenv'# Appelle la gem Dotenv

		Dotenv.load('.env') # Ceci appelle le fichier .env (situé dans le même dossier que le programme Ruby) grâce à la gem Dotenv, et importe toutes les données enregistrées dans un hash ENV

		# Il est ensuite très facile d'appeler les données du fichier .env, par exemple là je vais afficher le contenu de la clé TWITTER_API_SECRET
		puts ENV['TWITTER_API_SECRET']

		# tout est stocké dans un hash qui s'appelle ENV. Tu peux le regarder en faisant :
		puts ENV