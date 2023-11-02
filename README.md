# git_assignment_HeroVired
git_assignment_HeroVired - Assignment Repository created by Sunil Gaddi

Steps Followed:
git clone <repository_url>

cd git_assignment_HeroVired

git add calculator.py
git commit -m "Add initial calculator code"
git push origin dev

git tag -a v1.0 -m "Version 1.0 release"
git push origin v1.0

git checkout -b feature/sqrt

def square_root(self, x):
    return math.sqrt(x)

git add calculator.py
git commit -m "Add square root feature"

git checkout dev

def divide(self, a, b):
    if b == 0:
        raise ValueError("Cannot divide by zero.")
    return a / b

git add calculator.py
git commit -m "Fix divide function"

git push origin feature/sqrt

git tag -a v2.0 -m "Version 2.0 release"
git push origin v2.0

