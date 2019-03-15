# how to build release version
1. Run docker-compose
2. Enter to container
3. Check DIR-path at `/go/src/app`
4. build app : `env GOOS=linux GOARCH=arm GOARM=7 go build -o /home/release/app`
    - If raspi cpuinfo mode name is `arm71`, GOARM=7
5. Move `app` to raspberry-pi
