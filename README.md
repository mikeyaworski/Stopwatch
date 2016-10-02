# Stopwatch

## Overview
This is a Java object that simulates using a stopwatch.

## Usage

Just download this class and paste it directly into your project. Then instantiate the class and start calling the methods.

## Methods

- `void start()` Starts the stopwatch.
- `void stop()` Stops the stopwatch.
- `void reset()` Stops the stopwatch and resets the duration back to 0.
- `void restart()` Restarts the stopwatch by calling reset() and then start(). Resets the stopwatch back to 0 and then starts it again.
- `void getMilliseconds()` Returns the duration of the stopwatch as a long, in milliseconds. The duration starts when the stopwatch is first started using start() and is finished when the stopwatch is lastly stopped using stop(), or when this method is called if the stopwatch was not stopped since most recently started.
- `void getSeconds()` Returns the duration of the stopwatch as a double, in seconds. The duration starts when the stopwatch is first started using start() and is finished when the stopwatch is lastly stopped using stop(), or when this method is called if the stopwatch was not stopped since most recently started.
- `void getMinutes()` Returns the duration of the stopwatch as a double, in minutes. The duration starts when the stopwatch is first started using start() and is finished when the stopwatch is lastly stopped using stop(), or when this method is called if the stopwatch was not stopped since most recently started.
- `void isGoing()` Returns whether or not the stopwatch is currently active (has been started but not stopped since the most recent start() call).

## Examples

```java
Stopwatch stopwatch = new Stopwatch();

stopwatch.start();

// your code

stopwatch.stop();

System.out.println("Your code took " + stopwatch.getMilliseconds() + " milliseconds to execute.");
```