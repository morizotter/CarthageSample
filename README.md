# CarthageSample
Sample for publishing.

## How to install this sample repository

```bash
$ brew update
$ brew install carthage
$ cd /to/your-project-root/
$ vi Carthage
# Write one line below.
github "morizotter/CarthageSample"
$ carthage update
```

After above, read the documentation: [Adding frameworks to an application](https://github.com/Carthage/Carthage/blob/master/README.md#adding-frameworks-to-an-application).

Open your project and write `import CarthageSample` at the top of swift file where you want to test this sample. And write:

```swift
let sample = Sample()
sample.log() // sample
```

Done.
