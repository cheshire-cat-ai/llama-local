# llama-local for the Cheshire Cat AI (NVIDIA only)

This is an adaptation of llama-cpp-python (link) to be easily launched from docker-compose and with an NVIDIA GPU.


Clone repo: 

```
git clone https://github.com/cheshire-cat-ai/llama-local.git
```

Create your `.env` based on the provided example:

```
cp .env.example .env
```

Download the model of your choice (GGML format, many LLAMA versions are available [here](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML))

Place your `.bin` model in the `models` folder

MODEL_NAME in .env should match the filename of your LLAMA.

Launch the container:

```
docker compose up
```

Now go to [`http://localhost:8000/docs`](http://localhost:8000/docs) to try out the endpoints

TODO: instructions on how to configure the cat
