# Godot
```bash
flatpak remote-add --if-not-exists --user flathub https://dl.flathub.org/repo/flathub.flatpakrepo

flatpak install flathub org.godotengine.Godot -y
```

# Spack
```bash
git clone --depth=2 --branch=releases/v0.23 https://github.com/spack/spack.git ~/spack
cd ~/spack

. share/spack/setup-env.sh

spack install python@3.11
```
