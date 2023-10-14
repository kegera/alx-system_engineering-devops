# README

## Description

This repository contains various Ruby scripts for working with regular expressions. Each script focuses on specific regular expression patterns and their applications.

## Files

- `0-simply_match_school.rb`: Matches the word "School" in the given input.
- `1-repetition_token_0.rb`: Implements a basic repetition token regular expression.
- `2-repetition_token_1.rb`: Implements another repetition token regular expression.
- `3-repetition_token_2.rb`: Implements a more complex repetition token regular expression.
- `4-repetition_token_3.rb`: Implements an advanced repetition token regular expression.
- `5-beginning_and_end.rb`: Matches patterns that start and end with the same character.
- `6-phone_number.rb`: Matches phone numbers in different formats.
- `7-OMG_WHY_ARE_YOU_SHOUTING.rb`: Matches words with all uppercase letters.

## Usage

To make these scripts executable, use the following command:

```bash
chmod +x *.rb
After making the files executable, you can run them using the following syntax:
./<script_name>.rb <input_string>
Example:

sylvain@ubuntu$ ./0-simply_match_school.rb School | cat -e
School$
sylvain@ubuntu$ ./0-simply_match_school.rb "Best School" | cat -e
School$
sylvain@ubuntu$ ./0-simply_match_school.rb "School Best School" | cat -e
SchoolSchool$
sylvain@ubuntu$ ./0-simply_match_school.rb "Grace Hopper" | cat -e
$

Replace <script_name> with the name of the script you want to run
 and <input_string> with the input you want to test against the regular expression.
