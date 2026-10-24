# The Lord of the Rings Survey

A survey form about The Lord of the Rings, built for the freeCodeCamp **Survey Form** project (Responsive Web Design certification).

This is one of my first HTML projects. I'm still learning, so this README explains what I did, the problems I had and how I solved them.

## About the project

The goal of the lab was to build a survey page with a form and make all **44 tests** pass. The example project was a generic survey, so I chose my own theme: **The Lord of the Rings**. The tests only check the structure of the form, so any theme works.

## What's inside

- `index.html` - the page and the form
- `index.css` - the styles (work in progress)

## Form fields

| Field | Element | Notes |
|-------|---------|-------|
| Name | `input type="text"` | required, has a placeholder |
| Email | `input type="email"` | required, the browser checks the format |
| Number | `input type="number"` | how many times you watched the movies, `min="1"` and `max="20"` |
| Favorite character | `select` | 6 options (Frodo, Aragorn, Gandalf...) |
| Book or movie | `input type="radio"` | 2 radio buttons with the same `name` |
| Favorite places | `input type="checkbox"` | 10 places, each one with a `value` |
| Comments | `textarea` | optional |
| Submit | `button type="submit"` | "send to Rivendell" |

## How I built it

1. **Read the user stories and tests first.** I translated them to understand every requirement and made a checklist from the 44 tests.
2. **Chose the theme.** I picked The Lord of the Rings because it's fun and I can make a nice style for it later.
3. **Wrote the basic HTML structure:** `<!DOCTYPE html>`, `head` (charset, viewport, description, title, stylesheet) and `body`.
4. **Added the title and the description:** `h1#title` and `p#description`.
5. **Added the form:** `form#survey-form`. Everything else goes **inside** this one form.
6. **Added name, email and number** with their labels (`name-label`, `email-label`, `number-label`) and placeholders.
7. **Added the `select`** with `id="dropdown"` and the options.
8. **Added the radio buttons** with the same `name`, so only one can be chosen.
9. **Added the checkboxes**, all with the same `name` and a different `value`.
10. **Added the `textarea` and the submit button.**
11. **Checked the code test by test** until I had 44 out of 44.

## Problems I had and how I solved them

**1. Two different "descriptions".**
I thought the `description` was for SEO. I found out there are two things with the same name:
- `<p id="description">` is visible in the page and is required by the tests.
- `<meta name="description">` is in the `head`, is used by search engines and is not required by the tests.
I used both.

**2. Label and input were on the same line.**
`label` and `input` are inline elements, so they stay side by side. I fixed it by putting each label + input pair inside a `div`. I could also use `display: block` in CSS, but I'll decide when I do the styling.

**3. Where do the other fields go?**
At first I thought I needed a new form for every question. Wrong: there is **only one form**, and every new field goes inside it.

**4. Duplicate ids.**
Ids must be unique in the whole page, so I can't use `dropdown` twice. The `name` is different: radio buttons of the same question **must** share the same `name`, and checkboxes of the same question usually share it too. Different question = different `name`.

**5. Radio buttons and checkboxes need a `value`.**
Some tests check that every radio and checkbox has a `value` attribute, so I added one to each (for example `value="moria"`).

**6. The textarea went on the same line as its label.**
`textarea` is inline too. I wrapped it in a second `div`, so it goes under the question.

**7. Small spelling mistakes.**
The title was "The Lord of Rings", the correct name is **The Lord of the Rings**. I also learned that `example.com` is the domain meant for examples, so I used `frodo@example.com` in the email placeholder.

## My code style

- If an element has 2 attributes or fewer, I write it on one line.
- If it has more than 2, I write one attribute per line.
- All the code (text, names, comments) is in English.

## Things I learned

- The difference between inline and block elements
- Why ids must be unique and how `name` groups radio buttons
- HTML5 validation (`required`, `type="email"`, `min` and `max`) works without JavaScript
- How `label for="..."` connects to the `id` of an input
- The two kinds of "description" (visible text and SEO meta tag)

## What's next

- [ ] Write the CSS (parchment / Middle-earth style, serif font, centered form)
- [ ] Put the radio buttons and checkboxes in a nicer layout
- [ ] Add `name="name"` and `name="email"` to the first two inputs
- [ ] Try `fieldset` and `legend` for radio and checkbox groups
- [ ] Publish the project on GitHub

## Credits

Project idea and tests from [freeCodeCamp](https://www.freecodecamp.org/). The theme, the questions and the code are mine, and I used Claude as a study helper to understand the problems and check my work.
