[
    {
        "id": "23677dc8.1232e2",
        "type": "tab",
        "label": "Flow 2",
        "disabled": false,
        "info": ""
    },
    {
        "id": "a69702dc.ebfe3",
        "type": "tab",
        "label": "Flow 3",
        "disabled": false,
        "info": ""
    },
    {
        "id": "529d5327.592d0c",
        "type": "tab",
        "label": "Flow 1",
        "disabled": false,
        "info": ""
    },
    {
        "id": "3d528d98.966fc2",
        "type": "http in",
        "z": "529d5327.592d0c",
        "name": "",
        "url": "/pin4",
        "method": "get",
        "upload": false,
        "swaggerDoc": "",
        "x": 90,
        "y": 140,
        "wires": [
            [
                "303c135a.bd919c"
            ]
        ]
    },
    {
        "id": "8d745b35.de1558",
        "type": "rpi-gpio in",
        "z": "529d5327.592d0c",
        "name": "gpio4",
        "pin": "7",
        "intype": "up",
        "debounce": "25",
        "read": true,
        "x": 100,
        "y": 240,
        "wires": [
            [
                "cfe19f31.59439"
            ]
        ]
    },
    {
        "id": "cfe19f31.59439",
        "type": "function",
        "z": "529d5327.592d0c",
        "name": "set GPIO",
        "func": "global.set(\"GPIO\", msg.payload);\nreturn msg;",
        "outputs": 1,
        "noerr": 0,
        "x": 290,
        "y": 260,
        "wires": [
            [
                "c158f22.d17df1"
            ]
        ]
    },
    {
        "id": "303c135a.bd919c",
        "type": "function",
        "z": "529d5327.592d0c",
        "name": "Get GPIO",
        "func": "msg.payload=global.get(\"GPIO\");\nreturn msg;",
        "outputs": 1,
        "noerr": 0,
        "x": 260,
        "y": 140,
        "wires": [
            [
                "daa56ef8.d2105",
                "c158f22.d17df1"
            ]
        ]
    },
    {
        "id": "c158f22.d17df1",
        "type": "debug",
        "z": "529d5327.592d0c",
        "name": "",
        "active": true,
        "tosidebar": true,
        "console": false,
        "tostatus": false,
        "complete": "false",
        "x": 540,
        "y": 220,
        "wires": []
    },
    {
        "id": "daa56ef8.d2105",
        "type": "http response",
        "z": "529d5327.592d0c",
        "name": "",
        "statusCode": "",
        "headers": {},
        "x": 480,
        "y": 140,
        "wires": []
    }
]
