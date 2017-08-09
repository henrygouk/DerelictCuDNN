DerelictCuDNN
=============

Dynamic bindings to cuDNN for the D programming language.

Usage
-----

Similar to other Derelict-based dynamic bindings, simply call ```DerelictCuDNN.load()``` and begin using cuDNN!

```
    import std.conv : to;
    import std.stdio : writeln;
    import derelict.cudnn;

    void main(string[] args)
    {
        DerelictCuDNN.load();

        writeln(cudnnGetErrorString(CUDNN_STATUS_SUCCESS).to!string);
    }
```