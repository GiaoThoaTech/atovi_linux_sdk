# Atovi Linux SDK
> This is SDK to intergrate Atovi Smart Lock to Linux system 

## Table of contents

1. [Prerequisites](#prerequisites)
2. [Setup](#setup)
3. [Usage](#usage)
   1. [Unlock](#unlock)
   2. [Lock](#lock)
   3. [Check lock status](#check-lock-status)
4. [Support](#support)
6. [License](#license)

## Prerequisites
### Current Device support
`Raspberry Pi 3, Raspberry Pi zero w`

### Lock Use
[Atovi Lock](https://atovi.vn)

### Software
- python 3
- [bluepy](https://github.com/IanHarvey/bluepy)

## Setup
#### Step 1
Download `atovi_service.py` (contact tech@giaothoatech.com)
#### Step 2
Copy file `atovi_service.py` you have just download and paste it in your project directory

#### Step 3

in your app, import AtoviService
```python
from atovi_service import AtoviService
```
## Usage
### Unlock

```python
# lock_address: (string) Mac address of Atovi Smart Lock
# key: (int) lock key
AtoviService.shared().unlock(lock_address, key)
```
### Lock

```python
# lock_address: (string) Mac address of Atovi Smart Lock
# key: (int) lock key
AtoviService.shared().lock(lock_address, key)
```

### Check lock status

```python
# lock_address: (string) Mac address of Atovi Smart Lock
# key: (int) lock key
status = AtoviService.shared().status(lock_address, key)
```

## Support
drop an email to tech@giaothoatech.com for more info

## License
Copyright 2017 Atovi Smart Lock

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WaarANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.



