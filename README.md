from flask import Flask, json, jsonify, request

app = Flask(__name__)

items = []

@app.route('/trung_kiet', methods=['POST'])
def trung_kiet():
    json_data = request.json

    print(json_data)

    return 'Loged in successfully!', 200

if __name__ == '__main__':
    app.run(debug=True)
