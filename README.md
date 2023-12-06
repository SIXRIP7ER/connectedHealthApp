# README.md

# Pulling from github

First clone then retrieve submodules

```
git clone https://github.com/SIXRIP7ER/connectedHealthApp.git
cd connectedHealthApp/
git submodule update --init
```

# Docker Command to start

1. get ConnectionCode:

```
./getip
```

2. run docker:

```
docker-compose up
```

3. stop docker:

```
docker-compose down -v --rmi 'all'
```

# Inside Expo App : Patient

1. Download Expo App on smartphone
2. Follow link:

```
exp://ConnectionCode:19000
```

3. Enter for connection code in app.

```
ConnectionCode:8000
```

4. Press record button once and allow permission for recording for the first time, small delay before recording starts.

5. Press record again to stop recording, session id and session clip should be printed in the back-end

# Inside Web App : Staff

1. Access web app via:

```
http://ConnectionCode:8000/data/visualise2D/
```

2. use session id and clip num to view recordings.
