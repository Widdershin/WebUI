# flask-desktop

flask-desktop is a Python module that allows you to convert Flask apps into cross platform desktop apps with three lines of code.

## Installation:

```
pip install webui
```


## Usage:

```python

    from webui import WebUI # Add WebUI to your imports
    from flask import Flask, render_template, request

    app = Flask(__name__)
    ui = WebUI(app, debug=True) # Create a WebUI instance

    # all of your standard flask logic

    if __name__ == '__main__':
      ui.run() #replace app.run() with ui.run(), and that's it
```

flask-desktop is powered by PyQt5, and should run on Windows, Mac and Linux. You can even create standalone executables using PyInstaller!

## License

flask-desktop is licensed under the MIT License. See the LICENSE file for more details.
