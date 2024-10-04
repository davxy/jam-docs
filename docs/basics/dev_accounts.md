---
id: Dev Accounts
sidebar_label: Dev Accounts
---

:::warning

Never use these accounts with real funds.

:::

These well known accounts can be used for testing and are known by all JAM node implementations.

## Seeds

The 256 bit seeds for the dev accounts are generated by encoding the index of the validator and keeping the remaining bytes zero.

With the following indices for the accounts:

| Name   | Index |
|--------|-------|
| Alice  | 0     |
| Bob    | 1     |
| Carol  | 2     |
| David  | 3     |
| Eve    | 4     |
| Fergie | 5     |

**Pseudocode** to generate the first 2^32 seeds:
`0x00000000000000000000000000000000000000000000000000000000 ++ CodecEncodeU32(index)`

## Alice

```yaml
seed: 0x0000000000000000000000000000000000000000000000000000000000000000
ed25519_private: 0x00000000000000000000000000000000000000000000000000000000000000003b6a27bcceb6a42d62a3a8d02a6f0d73653215771de243a63ac048a18b59da29
ed25519_public: 0x3b6a27bcceb6a42d62a3a8d02a6f0d73653215771de243a63ac048a18b59da29
```

## Bob

```yaml
seed: 0x0000000000000000000000000000000000000000000000000000000000000001
ed25519_private: 0x00000000000000000000000000000000000000000000000000000000000000014cb5abf6ad79fbf5abbccafcc269d85cd2651ed4b885b5869f241aedf0a5ba29
ed25519_public: 0x4cb5abf6ad79fbf5abbccafcc269d85cd2651ed4b885b5869f241aedf0a5ba29
```

## Carol

```yaml
seed: 0x0000000000000000000000000000000000000000000000000000000000000002
ed25519_private: 0x00000000000000000000000000000000000000000000000000000000000000027422b9887598068e32c4448a949adb290d0f4e35b9e01b0ee5f1a1e600fe2674
ed25519_public: 0x7422b9887598068e32c4448a949adb290d0f4e35b9e01b0ee5f1a1e600fe2674
```

## David

```yaml
seed: 0x0000000000000000000000000000000000000000000000000000000000000003
ed25519_private: 0x0000000000000000000000000000000000000000000000000000000000000003f381626e41e7027ea431bfe3009e94bdd25a746beec468948d6c3c7c5dc9a54b
ed25519_public: 0xf381626e41e7027ea431bfe3009e94bdd25a746beec468948d6c3c7c5dc9a54b
```

## Eve

```yaml
seed: 0x0000000000000000000000000000000000000000000000000000000000000004
ed25519_private: 0x0000000000000000000000000000000000000000000000000000000000000004fd50b8e3b144ea244fbf7737f550bc8dd0c2650bbc1aada833ca17ff8dbf329b
ed25519_public: 0xfd50b8e3b144ea244fbf7737f550bc8dd0c2650bbc1aada833ca17ff8dbf329b
```

## Fergie

```yaml
seed: 0x0000000000000000000000000000000000000000000000000000000000000005
ed25519_private: 0x0000000000000000000000000000000000000000000000000000000000000005fde4fba030ad002f7c2f7d4c331f49d13fb0ec747eceebec634f1ff4cbca9def
ed25519_public: 0xfde4fba030ad002f7c2f7d4c331f49d13fb0ec747eceebec634f1ff4cbca9def
```

... there are 2^256 dev accounts in total that continue in the same pattern but are unnamed.