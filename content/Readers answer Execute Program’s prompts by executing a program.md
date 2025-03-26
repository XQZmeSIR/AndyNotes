# Readers answer Execute Program’s prompts by executing a program

Like the [[Mnemonic medium]], Execute Program’s lessons interleave prose with interactive prompts. But the central conceit which gives Execute Program its namesake is that every interaction involves executing a program inside an embedded interpreter. In fact, [[Execute Program doesn’t have non-executable prompts]].

For instance, a lesson might include several paragraphs introducing the notion that in SQL, you can select only a specific column by using `SELECT column_name`. Then it might offer this prompt:

    
    
exec(`CREATE TABLE cats (name STRING, age INTEGER)`); exec(`INSERT INTO cats (name, age) VALUES (“Boromir”, 3), (“Aragorn”, 15)`); exec(`SELECT name FROM cats`) >

The reader’s cursor is positioned on the final line; they’re meant to enter what the expression on the first line will evaluate to. Execute Program then evaluates the reader’s input expression (i.e. as Javascript) and compares the resulting value to the test value.

This _looks_ like a Quizlet-style flashcard, in which one must type in the correct answer, but it’s not. It’s a real interpreter, which will really evaluate your program. So you can write `[{name: “Boromir”}, {name: “Aragorn”}]` or `[“Boromir”, “Aragorn”].map(n => ({name: n})`—both are correct. I like that this design model puts the lessons closer to an authentic context: [[Enabling environments focus on doing what’s enabled]].

More complex prompts, called “problems,” provide readers with a source listing and a “goal expression”—the desired value for the last line. For example:

    
    
function adds2(input: number) { } adds2(4)
    
// GOAL: 6

The reader is meant to modify the source listing so that the goal expression is produced. When the reader’s ready, they execute their program; it’s evaluated and its output is compared to the goal value.

A related, more ambitious conceit: [[What might it mean to situate games like Shenzhen I/O inside pro environments like an IDE?]]

Also related: [[Executable books]]

* * *

Q. Execute Program’s prompts ask readers to input an answer. How is this interaction different from Quizlet’s? A. The answer is evaluated in a real interpreter, not just compared verbatim.

Q. Why does it matter that readers’ answers to Execute Program’s prompts are evaluated, not just compared verbatim? A. It allows readers some authentic flexibility in solving the prompts.

* * *
