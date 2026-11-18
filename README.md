# dev86 mirror archive

A mirror of one revision of [dev86](https://codeberg.org/jbruchon/dev86)
(the `bcc` C compiler, `as86` assembler and `ld86` linker for 8086 code),
kept so that builds pinned to that revision do not depend on the upstream host
being reachable. dev86 is licensed under the GNU General Public License,
version 2; see [COPYING](COPYING). This repository changes nothing in it.

The [v1.0.1 release](../../releases/tag/v1.0.1) carries
`dev86-0b72e907f7a282aaa777a768b8b688e41c77fc93.git.tar.gz`: a shallow bare git repository
(`dev86.git`) holding exactly upstream commit
`0b72e907f7a282aaa777a768b8b688e41c77fc93` (tag `v1.0.1`), with every file of
that revision.

| | |
| --- | --- |
| Upstream | https://codeberg.org/jbruchon/dev86 |
| Commit | `0b72e907f7a282aaa777a768b8b688e41c77fc93` |
| Tree | `9f40636a9a995ec892055fe953f1f70e50fe7551` |
| Archive SHA-256 | `f96e95431f47f14b3086f8e3e7fe3e844c8c130e45ab800bbc88a0a013a1f4c2` |

Git verifies the commit when it is fetched from the unpacked repository:

```sh
tar -xzf dev86-0b72e907f7a282aaa777a768b8b688e41c77fc93.git.tar.gz
git init dev86 && cd dev86
git fetch --depth 1 "file://$PWD/../dev86.git" 0b72e907f7a282aaa777a768b8b688e41c77fc93
git checkout FETCH_HEAD
```

The upstream history is not here: the archive was made from a depth-1 clone.
