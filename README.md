##### 1. What's the output?

```javascript
  2 + 0 || [3,4][1] || 5 || ""
```

- A: `"2"`
- B: `6`
- C: `2`
- D: `NaN`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

The line is equal to `(2 + 0) || [3,4][1] || 5 || ""`. `||` operator getting the first truthy value from a list of variables or expressions.

</p>
</details>

##### 2. What's the output?

```javascript
  4 && 2 + 9 - 11 && 3
```

- A: `0`
- B: `2`
- C: `14`
- D: `3`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

The line is equal to `4 && (2 + 9 - 11) && 3`. `&&` operator returns the first falsy value or the last value if none were found.

</p>
</details>

##### 3. What's the output?

```javascript
  2 + (0 || [3,4][1] || 5 || "")
```

- A: `2`
- B: `6`
- C: `5`
- D: `7`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: B

The line is equal to `2 + [3,4][1]`. `||` operator getting the first truthy value from a list of variables or expressions.

</p>
</details>

##### 4. What's the output?

```javascript
  2 + 9 - 11 || [3,4][2] || 5 || ""
```

- A: `""`
- B: `5`
- C: `0`
- D: `4`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: B

The line is equal to `0 || undefiend || 5 || ""`. `||` operator getting the first truthy value from a list of variables or expressions which is `5`.

</p>
</details>

##### 5. What's the output?

```javascript
  4 && 2 + 9 - 11 && 3 || [3,4][2] || 5 || ""
```

- A: `4`
- B: `""`
- C: `5`
- D: `14`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

The line is equal to `(4 && 2 + 9 - 11 && 3) || [3,4][2] || 5 || ""`. The first expresion returns 0 as `&&` operator returns the first falsy value or the last value if none were found, and the `||` operator getting the first truthy value from a list of variables or expressions which is `5`.

</p>
</details>