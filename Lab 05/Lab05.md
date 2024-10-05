## Lab 05

- Name: Dan Gnau
- Email: gnau.11@wright.edu

## Part 1 

Make sure the following files are in your GitHub repository
- validator (with commits for each step complete)
- `clean1.txt` through `clean4.txt`

## Part 2 Answers

1. `sed 's/<\/[^>]*>//g'`
2. `sed 's/[[:space:]]*<li>/- /g'`
3. `sed 's/<h1>\(.*\)<\/h1>/# \1/g'`
4. `sed 's/<h2>\(.*\)<\/h2>/## \1/g'`
5. `sed 's/<ul>//g; s/<\/ul>//g; s/<html>//g; s/<\/html>//g'`
6. `sed 's/\bBatches\b/Matches/g'`

## Part 3 Answers

1. `awk '$1 ~ /^Bil/ {print $1}' records.txt`
2. `awk '$4 == 42 {print $3}' records.txt`
3. `awk '$3 ~ /wright\.edu/ {print $2 ", " $1 ": " $3}' records.txt`
4. `awk '$3 ~ /wright\.edu/ && $5 == "1234" {print $2 " favorite number is: " $4}' records.txt`
5. `awk '{$5 = "N0T@PL@!NP@$$W0RD"; print}' records.txt > updaterecords.txt`

## Extra Credit - Remove this if not doing

1. Source: [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions](https://html.spec.whatwg.org/multipage/input.html#valid-e-mail-address)
    - Regular Expression Pattern: /^[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$/
2. Pattern explanation:
   -Starts with valid characters, followed by an @.
    -Contains a domain that starts with an alphanumeric character, can have hyphens, and allows for multiple subdomains.
    -Ends with a valid structure, ensuring it conforms to common email formatting rules.
4. Verify `validator2` is in your GitHub repository
