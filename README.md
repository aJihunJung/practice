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
  // 필요한 라이브러리 설치
  $ sudo apt-get install git curl libcurl4-openssl-dev libpq-dev nodejs -y
  
  //rvm(ruby version manager) 설치
  $ gpg --keyserver hkp://keys.gnupg.net --recv-keys D39DC0E3 
  $ \curl -L https://get.rvm.io | bash -s stable
    * RVM 설치 방법에는 2가지가 있다.
      - single user install
        + 설치한 유저에게만 rvm이 설치
        + 설치한 rvm은 해당유저만 사용가능하고, 다른 유저가 사용할 수 없다.
        + rvm은 설치한 유저의 홈 디렉토리의 .rvm폴더($HOME/.rmv)에 설치된다.(rvm 으로 설치하는 ruby, gem등도 모두  해당 폴더에 저장)
        + root계정으로 single user install을 할 수 없다.
      
      - multi user install
        + /usr/local/rvm/에 모든 rvm, ruby, gem이 설치된다.
        + 한 유저가 설치한 ruby, gem이 시스템 전체에공유된다.
        + rvm그룹의 유저만 새루비 또는 gem을 설치할 수 있다.
  
  //rvm access
  $ source ~/.rvm/scripts/rvm
  
  //Dependence 해결 - ruby, rails등이 OS따라 의존성 업데이트
  $ rvm requirements
  
  //ruby install
  $ rvm install 2.1.0 [version] (rvm reinstall 2.1.0 : 기존에 설치된 바이너리 삭제후 재설치)
  $ rvm use 2.1.0 --default
  
  //gem update
  $ rvm rubygems current
  
  //rails 설치
  $ gem install --no-ri --no-rdoc rails
    - 설치된 rails version 확인 : $ gem list --local rails
    - 원하는 rails version 설치 : $ gem install rails --version [version]
    - '--no-ri' '--no-rdoc' default setting : vi ~/.gemrc -> gem: --no-ri --no-rdoc 
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

