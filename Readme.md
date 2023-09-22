# Assignment 2

This package is a jsonapi that allows for the json serialization and deserialization of complex numbers and range.

To install, download the folder and run the project with "python -m build" to create a tarfile and wheel

Given a complex number, our api will call encode/decode complex which returns the following:


    def decode_complex(self, obj):
        return complex(obj["real"], obj["imag"])
    def encode_complex(self, c):
        return {"real": c.real, "imag": c.imag}

