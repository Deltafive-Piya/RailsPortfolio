# README

Ruby on Rails Deployed Porfolio Page.

* rails new RailsPortfolio --api --database=postgresql --skip-webpack-install --skip-action-mailbox --skip-action-mailer --skip-action-text --skip-spring --skip-turbolinks --skip-system-test

Parallax (ONLY CSS)

<img src="/piyaUpdates/rordojo.png" alt="A snapshot of the current Project">
<img src="/piyaUpdates/rordojo-inspect.png" alt="A snapshot including the inspect section">

* Issues encountered so far:
  * (console) run as admin
* <a href="https://www.postgresql.org/download/"> **PSQL**
  * <a href="https://www.pgadmin.org"> **pgAdmin**
* -**pg_ctl start**-no database directory specified and environment variable PGDATA unset--
  * gem install pg ~> bundle install ~> bundle update ~> pg_ctl start ~> pg_ctl status
* <a href="https://chocolatey.org"> **Choco**
* <a href="https://www.enterprisedb.com/downloads/postgres-postgresql-downloads"> **introduce psql for db**
  * Altering **database.yml** for postgres authentication prior to **'rails db:create'**.
  * postgresql db w/o auth- converting "scram-sha-256" to "trust" @ pg_hba.conf <~~THIS SOLVED AUTH ISSUE, FOR NOW
    * pg_ctl start -> pg_ctl status ~> rails s
* use the chown command with your username to change the ownership. Use the following command:
    *  "chown -R <username> ."
*  application.bootstrap.css asset was not declared to be precompiled in the production environment.
    * //= link application.bootstrap.css 
* **Formatting In Guthub Readme?!?!**

Things you may want to cover:
* System dependencies
  * Gem -v<a href="https://blog.rubygems.org/2022/02/09/3.3.7-released.html"> **3.3.7**
  * Ruby -v<a href="https://www.ruby-lang.org/en/news/2022/04/12/ruby-3-1-2-released/">  **3.1.2**
  * Rails -v<a href="https://rubygems.org/gems/rails/versions/3.1.2">  **7.0.6**
    * Configuration <br>
        "Bundle"/"Bundle install"
        (path for Dojonary view = http://localhost:XXXX/home/index)
    * DB creation & initialization
        "db:create & db:migrate..."
    * Deployment instructions
        <a href="https://guides.rubyonrails.org/command_line.html">  pg_ctl start **THEN** Rails S</a>
    * ...
  * <a href="http://127.0.0.1:54420/help/help/preferences.html"> **PGAdmin dark**
