# Creating a console App

To create a dart console app we can use the `dart create` command.

For example:
```sh
# Creating a console app name helloworld
dart create -t console helloworld
```

## Run the generated console app

The sample console app created will indeed be a Hello World app with a twist, it will call the `calculate()` function and print the number returned.

To run the app created with the previous sample code use the `dart run` command:
```sh
# Move to the helloworld directory
cd helloworld

# Run the app
dart run
```

## Compile the native executable binary file

The run command used previously will run the app using the Dart VM.

If you want to generate a binary you need to compile the console application with the `dart compile` command.
```sh
# Compile the helloworld.dart source code
dart compile exe bin/helloworld.dart

# Use this on a linux machine to avoid the .exe extension
dart compile exe bin/helloworld.dart -o bin/helloworld
```

Notice that when using the -o option we specified the bin directory to be the output directory.
This was done because when not using the -o option dart will put it on the bin directory. 
We wanted both commands to produce the same result, but you can also use `-o helloworld` and have the binary created on the current directory instead.

## Some useful links:

[Get Started with Command-Line Apps](https://dart.dev/tutorials/server/get-started)

[Introduction to Dart](https://dart.dev/language)

[Go Deeper: Dart Overview](https://dart.dev/overview)

[Effective Dart](https://dart.dev/effective-dart)
