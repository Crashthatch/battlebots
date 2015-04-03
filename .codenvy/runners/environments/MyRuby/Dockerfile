FROM codenvy/ruby210

ADD $app$/ /home/user

#Ruby dependencies (https://gorails.com/setup/ubuntu/14.04):
#RUN sudo apt-get install -q -y git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties
#Gosu dependencies (): 
#RUN sudo apt-get install -q -y build-essential libsdl2-dev libsdl2-ttf-dev libpango1.0-dev libgl1-mesa-dev libfreeimage-dev libopenal-dev libsndfile-dev;
#texplay dependencies:
#RUN sudo apt-get install -q -y freeglut3-dev

RUN sudo apt-get install -q -y ruby-dev;

RUN sudo gem install bundler

CMD bundle exec rtanque start bots/* sample_bots/camper sample_bots/seek_and_destroy sample_bots/keyboard;