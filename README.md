# README

## Ruby?

  ```nohighlight
  - Interpreter의 도움을 받아 실행되는 script language
  - Static한 type이 없는 dynamic language
  - Functional language
  - Object-oriented language
  ```

## Ruby on Rails(RoR)
  ```nohighlight
  - 웹개발을 MVC 구조로 제작
  - 반복되는 코드를 공용으로 쓸 수 있다
  - 자주 만드는 코드를 generate를 사용해서 만든다.
  - Object Releation Mapping 기능 제공
  - 반복되는 DB schema변경을 효율적으로 관리
  ```

## How to install ruby on rails

  ```nohighlight
  $ sudo apt-get update
  $ sudo apt-get install git curl libcurl4-openssl-dev libpq-dev nodejs -y
  $ gpg --keyserver hkp://keys.gnupg.net --recv-keys D39DC0E3 
  $ \curl -L https://get.rvm.io | bash -s stable
  $ source ~/.rvm/scripts/rvm
  $ rvm requirements
  $ rvm install 2.1.0
  $ rvm use 2.1.0 --default
  $ rvm rubygems current
  $ gem install --no-ri --no-rdoc rails
  ```

## How to craete new project

  ```nohighlight
  $ rails new [projectName]
   - Using Database : postgresql
  $ rails new [projectName] -db postgresql
  ```
  
## rails command
  ```nohighlight
  1. rails server (=rails s)
   - rails server 실행
   - option
    -e : default 개발환경
    -p : port 설정
    -b : ip Adress 설정
  ```

