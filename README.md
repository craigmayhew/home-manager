# home-manager

This is my MacOS nix [home manager](https://github.com/nix-community/home-manager) config. It's forked from [vaporif](https://github.com/vaporif/home-manager/) (Many thanks vaporif!).

I'm also using brew for a few items that are not yet via nix.

## setup

1. Clone this repo
2. Install [homebrew](https://brew.sh/)
3. Install packages via `brew bundle`
4. Install [nix](https://nixos.org/download) with [flakes](https://github.com/mschwaig/howto-install-nix-with-flake-support)
5. Install [home-manager](https://github.com/nix-community/home-manager)
6. Run the initial setup which will build all the derivations which may take a while. `nix flake`
7. Override home manager dir with this repo `ln -sf ~/Documents/GitHub/craigmayhew/home-manager ~/.config/nixpkgs`
8. for the first time `home-manager switch --flake ~/.config/nixpkgs --extra-experimental-features nix-command --extra-experimental-features flakes`
9. subsequent `home-manager switch`

## further reading
- https://nix.dev/recommended-reading
