# VS2022-PythonApplication1
Visual Studio 2022 Python Application

Default template for working with Python from Visual Studio 2022 Community Edition

To add pre-commit git pre-commit hook on tests, add hook and change it to executable

```bash
touch .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```

```bash
#!/bin/sh
set -e
cd "${0%/*}"
status=$?
../../bin/test.sh
status=$?
[ $status -eq 0 ] && echo "SUCCESS" || exit 1
```


![image 1](https://user-images.githubusercontent.com/383256/144722732-0b934168-f2e2-4de8-bc45-4c34765421c0.png)

![image 2](https://user-images.githubusercontent.com/383256/144722759-560f6dc5-8db1-4220-81c3-8ca27f71f64a.png)

![image 3](https://user-images.githubusercontent.com/383256/144722778-9dc58f4a-2a0a-40cb-a528-cf74af00ffa2.png)
