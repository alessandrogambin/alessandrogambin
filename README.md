### Hi there, I'm Alessandro 👋

#### I'm a:
- Software Engineer (SDE)
- Machine Learning, Deep Learning, and Data Science practitioner
- And a lifelong learner!

---
> If you set your goals ridiculously high and it's a failure, you will fail above everyone else's success. *- James Cameron*
---

```bash
~ » vi me.py█
```

```python
"""
Wait, does it seem a little empty, doesn't it?! 🤔
Yes, but just for a while... 🥳
I have a wide area of interest. 🤓
A lot of things are just coming! 😍
Come back later (you will not regret it). Engines are just starting to burn... 🚀
"""

from dataclasses import dataclass
from typing import Tuple


class Meta(type):

    def __new__(cls, name, bases, attrs):
        new_cls = super().__new__(cls, name, bases, attrs)

        return dataclass(unsafe_hash=True, frozen=True)(new_cls)


class Bio(metaclass=Meta):
    name        : str = "Alessandro Gambin da Silva"
    designation : str = "Software Engineer"
    base        : str = "Earth (remote work is life!)"


class Stack(metaclass=Meta):
    languages   : Tuple[str, ...] = ("JavaScript", "Python", "PHP")
    databases   : Tuple[str, ...] = ("MySQL", "PostgreSQL", "Mongo")
    misc        : Tuple[str, ...] = ("Linux", "Docker")
    ongoing     : Tuple[str, ...] = ("A lot! 🚀", "An advice: never stop learning!")


class Social(metaclass=Meta):
    linkedin    : str = "alessandrogambin"
    instagram   : str = "@alessandrogambin"
```
