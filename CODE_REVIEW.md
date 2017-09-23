# Code Review


## Everyone
* Be explicit. Remember people don't always understand your intentions online.
* Be humble. ("I'm not sure - let's look it up.")
* Don't use hyperbole. ("always", "never", "endlessly", "nothing")
* Don't use sarcasm.
* Ask for clarification. ("I didn't understand. Can you clarify?")
* Avoid selective ownership of code. ("mine", "not mine", "yours")
* Avoid using terms that could be seen as referring to personal traits. ("dumb", "stupid"). Assume everyone is intelligent and well-meaning.

## Reviewing Code
Understand why the change is necessary (fixes a bug, improves the user experience, refactors the existing code). Then:
* Communicate which ideas you feel strongly about and those you don't.
* Identify ways to simplify the code while still solving the problem.
* If discussions turn too philosophical or academic, move the discussion offline. In the meantime, let the author make the final decision on alternative implementations.
* Offer alternative implementations, but assume the author already considered them. ("What do you think about using a custom validator here?")
* Seek to understand the author's perspective.

## Having Your Code Reviewed

* Be grateful for the reviewer's suggestions. ("Good call. I'll make that change.")
* A common axiom is "Don't take it personally. The review is of the code, not you." We used to include this, but now prefer to say what we mean: Be aware of how hard it is to convey emotion online and how easy it is to misinterpret feedback. If a review seems aggressive or angry or otherwise personal, consider if it is intended to be read that way and ask the person for clarification of intent, in person if possible.
* Keeping the previous point in mind: assume the best intention from the reviewer's comments.
* Explain why the code exists. ("It's like that because of these reasons. Would it be more clear if I rename this class/file/method/variable?")
* Try to respond to every comment.
