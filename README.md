# FastAPI Project
This project is an example of a FastAPI Server. The project can be deploy and edited locally via VSCode or GitHub Codespaces.


## Deploy via Codespaces
In GitHub, pick Codespaces and create a codespaces. You will get a browser based VSCode.

### Setup
You can start by installing the following plugins to VSCode:
- Python by Microsoft

In the terminal, install the dependencies:
```bash
pip install -r requirements.txt
```

The terminal may ask to update pip, if so, you can run the following:
```bash
python3 -m pip install --upgrade pip
```

### Running
Finally, you can run the application with the following terminal command:
```bash
python3 -m uvicorn main:app --host 0.0.0.0 --port 8080
```

## Deploy FastAPI on Render

Use this repo as a template to deploy a Python [FastAPI](https://fastapi.tiangolo.com) service on Render.

See https://render.com/docs/deploy-fastapi or follow the steps below:

### Manual Steps

1. You may use this repository directly or [create your own repository from this template](https://github.com/render-examples/fastapi/generate) if you'd like to customize the code.
2. Create a new Web Service on Render.
3. Specify the URL to your new repository or this repository.
4. Render will automatically detect that you are deploying a Python service and use `pip` to download the dependencies.
5. Specify the following as the Start Command.

    ```shell
    uvicorn main:app --host 0.0.0.0 --port $PORT
    ```

6. Click Create Web Service.

Or simply click:

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/render-examples/fastapi)

### Thanks

Thanks to [Harish](https://harishgarg.com) for the [inspiration to create a FastAPI quickstart for Render](https://twitter.com/harishkgarg/status/1435084018677010434) and for some sample code!