# Countdown Timer

This project demonstrates a countdown timer using TypeScript and the `date-fns` library. The timer takes a user-defined number of seconds and counts down to zero, displaying the remaining time in minutes and seconds format.

## Features

- Prompts the user to input the number of seconds for the countdown.
- Validates the input to ensure it is a number and is within the valid range (0-60 seconds).
- Displays the remaining time in `MM:SS` format.
- Announces when the timer has expired.

## Dependencies

- [date-fns](https://date-fns.org/): A modern JavaScript date utility library.
- [inquirer](https://www.npmjs.com/package/inquirer): A library for creating interactive command-line interfaces.

## Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

## Usage

1. Run the countdown timer script:

   ```bash
   npx ts-node <script-file>.ts
   ```

2. Enter the number of seconds when prompted. The input should be a valid number between 0 and 60.

3. The script will display the countdown in `MM:SS` format every second until the timer expires.

## Code Explanation

- **Imports**
  - `differenceInSeconds`, `min`: Functions from `date-fns` to calculate time differences.
  - `inquirer`: Library for prompting user input.

- **User Input**
  - Prompts the user to enter the number of seconds.
  - Validates the input to ensure it's a valid number and within the range.

- **Countdown Logic**
  - Calculates the end time by adding the input seconds to the current time.
  - Uses `setInterval` to update the countdown every second.
  - Displays the remaining time in `MM:SS` format.
  - Exits the process when the timer reaches zero.

## Example

```plaintext
Please Enter the amount of seconds: 10
00:10
00:09
...
00:01
Timer has expired
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---


```
