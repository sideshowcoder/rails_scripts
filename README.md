Rails Scripts
=============
A collection of bash scripts I keep using for about every rails project. Just
drop in the rails scripts folder and run with it!

Dependecies
-----------
  * zeus (prefork env for rails to keep tests fast)
  * vagrant (vm managment tool)
  * expect-dev (contains unbuffered which is used to get colorized output over ssh)

test
----
Bash script to run rspec test correctly for a given environment, this is just an
extension of [Gary Bernhardts test
script](https://github.com/garybernhardt/destroy-all-software-extras/blob/master/das-0010-fast-tests-with-and-without-rails/test)
It handles the loading and execution of the specs for the right environment, be
it [zeus](https://github.com/burke/zeus) or [vagrant](http://www.vagrantup.com/)
and only load rails if it is needed to keep the tests fast.

start\_dev\_server
------------------
Start the development server managed by
[foreman](https://github.com/ddollar/foreman). Really simple but makes sure
foreman runs with Procfile.development.

License
-------
Released under the MIT license: http://opensource.org/licenses/MIT

