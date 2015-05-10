# CarthageSample
Sample for publishing.

### 0. Create Xcode project or workspace at the root directory

```bash
.
├── CarthageSample
├── CarthageSample.xcodeproj
└── CarthageSample.xcworkspace
```

### 1.Add target for framework

![framework](misc/00_framework.png)

### 2. Make Scheme shared

![schemes](misc/01_manage_schemes.png)

![shared](misc/03_shared.png)

### 3. Check building

```bash
$ carthage build --no-skip-current
```

Build with command above and check inside `Carthage/Build`.

### 4. git push

No problem? Then commit your changes and push it to github.

### 5. tag

Click release and add new tag for your commit.

![release](misc/04_release.png)

### 6. done

Use with `carthage` from another project!

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
