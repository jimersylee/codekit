# 1 - 切换镜像源
打开命令行并执行以下命令：

```bash
sed -i '1s|^|Server = {{link}}/$repo/os/$arch\n|' /etc/pacman.d/mirrorlist
```

# 2 - 更新镜像源缓存
打开命令行并执行以下命令：

```bash
pacman -Syy
```

# 3 - 开始使用
现在便可以正常使用 `pacman` 。

```bash
pacman -S <package name>
```