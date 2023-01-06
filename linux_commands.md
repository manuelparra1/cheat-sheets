# Installing Packages

---

## Install `sudo`

**Debian, Ubuntu**

```bash
apt install sudo
```

**Arch**

```bash
pacman -S sudo
```

**AlpineLinux**

```bash
apk add sudo
```

**Fedora**

```bash
dnf install sudo
```

# Common Tasks

---

## Adding User Account - `useradd`

**Ubuntu, Debian**

```bash
adduser dusts
passwd dusts
```

**Arch**

```bash
useradd -mpU dusts
```

## Adding `sudo` Privileges

**Ubuntu, Debian**

```bash
usermod -aG sudo dusts
```

**Arch**

```bash
useradd
```
