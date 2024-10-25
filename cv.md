# Sergei Goncharov

## 📲 Contact Info

Telegram: [@serezha_goncharov](https://t.me/serezha_goncharov)  
E-mail: [blist.zheleza@gmail.com](mailto:blist.zheleza@gmail.com)

## 🙋‍♂️ About Me

I have 3+ years of working with web as a QA Engineer,  
but I just get more fun to bring something new to the world,  
rather than check how others doing it.

## 💪 Skills

`Chrome Dev Tools`  
`Javascript`  
`HTML`  
`CSS`

`Cypress`

`Python`  
`Aiogram 3`  
`Telegram API`  
`PostgreSQL`  
`SQLite`  
`SQL Alchemy`  
`Docker`

`Agile/Scrum`  
`Confluence`  
`Jira`

## 👨‍💻 Code Examples

[Make the Deadfish Swim](https://www.codewars.com/kata/51e0007c1f9378fa810002a9)

```javascript
/**
 * Parser to interpret and execute the Deadfish language.
 *
 * It uses four single-character commands:
 * i: Increment the value
 * d: Decrement the value
 * s: Square the value
 * o: Output the value to a result array
 * All other instructions are no-ops and have no effect.
 *
 * Examples
 * parse("iiisdoso") should return numbers [8, 64].
 * parse("iiisdosodddddiso") should return numbers [8, 64, 3600].
 *
 * @param data - string with coded message
 * @type {(data: string) => Array}
 * @returns {Array}
 */
function parse(data) {
	const result = [];
	let counter = 0;
	const commands = data.split('');

	commands.forEach(command => {
		if (command === 'i') {
			counter = counter + 1;
		}
		if (command === 'o') {
			result.push(counter);
		}
		if (command === 's') {
			counter = counter ** 2;
		}
		if (command === 'd') {
			counter = counter - 1;
		}
	});

	return result;
}
```

[Simple Fun #47: Stolen Lunch](https://www.codewars.com/kata/58884a65f06a3d3bef000049)

```javascript
/**
 * Decoding message (note).
 * Decodes numbers into string and vice versa based on the rule below:
 *
 * Digit 0 is replaced with 'a',
 * 1 is replaced with 'b'
 * and so on, with digit 9 replaced by 'j'.
 *
 * @param note - string with coded message
 * @type {(note: string) => string}
 * @returns {string}
 */
function stolenLunch(note) {

	const noteArray = note.split('');
	const cipherMap = {
		"0": "a",
		"1": "b",
		"2": "c",
		"3": "d",
		"4": "e",
		"5": "f",
		"6": "g",
		"7": "h",
		"8": "i",
		"9": "j",
	};


	for (let i = 0; i < noteArray.length; i++) {
		// check if we have coded character in the note
		if (noteArray[i] in cipherMap) {
			// replace digit with corresponding letter
			noteArray[i] = cipherMap[noteArray[i]];

		}
		// check if we have decoded character in the note
		else if (Object.values(cipherMap).includes(noteArray[i])) {
			// replace letter with corresponding digit
			noteArray[i] = Object.keys(cipherMap).find(key => cipherMap[key] === noteArray[i]);

		}
	}

	return noteArray.join("");
}
```

## 👨‍🚀 Work Experience

QA Engineer with (3+ years)  
Customer support (2+ years)

## 📚 Education

- [HTML&CSS Crash Course](https://v2.scrimba.com/html-css-crash-course-c02l) by Kevin Powell
- [Learn Javascript](https://learn.javascript.ru/)
- [RS School](https://rs.school/courses/javascript-ru)

<span style="color:gray">* Background: Higher Education - Electrical engineer.</span>

## 🙊 Languages

- Russian: Native speaker
- English: Upper-Intermediate
- Chinese: Beginner

> Experience:   
> Finished language school with focus on English and Chinese  
> Lived abroad around 2 years in total  
> Worked in international / multicultural company for 2+ years
