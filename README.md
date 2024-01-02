
# Depth-Estimation App

End-to-end fundamental depth-estimation app 


## Usage/Examples

### CLI Usage

Flow  can be arbitrarily change by interacting with the cli.py file

```bash
usage: cli.py [-h] input_image output_image

Depth estimation using ZoeDepth.

positional arguments:
  input_image   Path to input image.
  output_image  Path to output depth map.

options:
  -h, --help    show this help message and exit
```
### API Usage

#### Bash Code to Redirecting API
```
uvicorn app:api

uvicorn app:api --reload
```

#### Local API Link
```
http://127.0.0.1:8041/predict

http://127.0.0.1:8041/docs
```
## Installation 

Install depth estimation project with pip

```bash
pip install -r requirements.txt
```
    
## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`IMG_API_KEY`

  
## Deployment

To deploy this project and run afterwards

```bash
docker build -t depth_estimation .
docker run -d -p 8041:8041 depth_estimation
```

  
## License

[MIT](https://choosealicense.com/licenses/mit/)

  