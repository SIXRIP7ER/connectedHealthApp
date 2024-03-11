# Pulling from github

First clone then retrieve front-end and back-end

```
git clone https://github.com/SIXRIP7ER/connectedHealthApp.git
cd connectedHealthApp/
git clone https://github.com/realRickyNguyen/ExpoCAMwithTensor.git
git clone https://github.com/nick-maiden/connectedhealth.git
```

## Running without Docker
1. If you wish to run the front-end manually without docker, access and follow instructions in the front-end repository
[Front-End](https://github.com/realRickyNguyen/ExpoCAMwithTensor).

2. If you wish to run the back-end manually without docker, access and follow instructions in the back-end repository
[Back-End](https://github.com/nick-maiden/connectedhealth).

Otherwise follow instructions below to run using docker.

# Running using Docker Method

1. get ConnectionCode (local IP address):

```
./getip
```

2. run docker:

```
docker-compose up
```

delete old docker build after making changes:

```
docker-compose down -v --rmi 'all'
```

# Inside Expo App : Patient

1. Download Expo App on smartphone
2. Follow link on browser: (Connection code is your local IP address not docker IP address)

```
exp://ConnectionCode:19000
```

3. Enter connection code (local IP-address) and back-end port inside app.

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
