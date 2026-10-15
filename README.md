# Iris: containerize a model and optimize it

    ./build_naive.sh        # steps 1-2
    ./measure.sh            # steps 3-5
    ./build_opt.sh          # step 4
    ./scan.sh               # step 7 (requires trivy)

## API + Redis login counter

    docker compose up --build -d
    ./test_api.sh
    docker compose logs api
    docker compose down          # add -v to also wipe the Redis counter

Endpoints: GET /health, POST /predict, POST /login, GET /stats
# Reddis-user-tracking
