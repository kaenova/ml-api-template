# ML API Template 🚀

Hello everyone! In this repository, I (Kaenova, a mentor in Bangkit 2023 program) will provide you with a head start on creating an ML API. Please read every line and comment carefully.

I have included code examples for both text-based input and image-based input APIs. To run this server, make sure to install all the required libraries listed in `requirements.txt` by executing the command `pip install -r requirements.txt`. Then, use the command `python main.py` to run the server.

## Machine Learning Setup

Please prepare your model in either the `.h5` or saved model format. Place your model in the same folder as the `main.py` file. You will load your model in the code provided below. There are two options available: one for image-based input and another for text-based input. You need to complete either the `def predict_text` or `def predict_image` functions in `main.py` based on your model's input type.

## Cloud Computing

You can check the endpoints used for the machine learning models in this API. The available endpoints are `/predict_text` for text-based input and `/predict_image` for image-based input. 

For the `/predict_text` endpoint, you need to send a JSON payload with the following structure:
```json
{
  "text": "your text"
}
```

For the `/predict_image` endpoint, you need to send a multipart-form with a field named "uploaded_file" containing the image file.

You can view the API documentation by accessing the `/docs` endpoint after running the server. Additionally, a Dockerfile is provided to facilitate modification and container image creation. By default, the server runs on port 8080, but you can customize the port by injecting the `PORT` environment variable.

## Consultation

If you need any assistance or would like to schedule a consultation with me, feel free to reach out to me on Discord (kaenova#2859). We can discuss your requirements and arrange a consultation time.

Finally, I encourage you to share your capstone application with me! You can connect with me on the following platforms:

- Instagram: [@kaenovama](https://www.instagram.com/kaenovama)
- Twitter: [@kaenovama](https://twitter.com/kaenovama)
- LinkedIn: [/in/kaenova](https://www.linkedin.com/in/kaenova)

Now, you can start writing your deploying your model. Happy coding!

---

## Usage

To get started, follow these steps:

1. Clone the repository:
```sh
git clone https://github.com/your-username/your-repository.git
```

2. Install the required libraries:
```sh
pip install -r requirements.txt
```

3. Prepare your machine learning model:
- If you have an `.h5` model file, place it in the same folder as `main.py`.
- If you have a saved model format, place it in a folder named `my_model_folder` in the same directory as `main.py`.

4. Read the `main.py` file carefully

5. Complete the `predict_text` or `predict_image` function in `main.py`

6. Run the server:
```sh
python main.py
```

---

## One More Thing

One thing i should mention. Many people still asking **Who should deploy the model? Is it CC or is it ML?**
> Both parties need to collaborate. Cloud Computing (CC) may not be familiar with the contents of your .h5 file, and Machine Learning (ML) may not be familiar with HTTP POST and GET requests. Therefore, it is the responsibility of both parties to deploy the model.
