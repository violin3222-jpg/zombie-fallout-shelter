[mashup-design.md](https://github.com/user-attachments/files/33244562/mashup-design.md)
# zombie-fallout-shelter
zombie-fallout-shelter
# Zombie Fallout Shelter: design sheets (v1)

Solo. Melty host: TBD (must be a game in Melty's catalog; check with search_games).
60 Seconds! Reatomized and Plants vs. Zombies: GOTY are both "secondary" (not in Melty's catalog): the mod finds each install folder itself, reads content from it, and shows an in-game message if either is missing. No look-alike assets.

## Sheet: phases
| id | name | duration | next | source |
|---|---|---|---|---|
| dash | Scavenge dash | 60s | wave1 | 60 Seconds rules |
| wave1 | Zombie wave 1 | until cleared | wave2 | PvZ rules |
| wave2 | Zombie wave 2 | until cleared | wave3 | PvZ rules |
| wave3 | Zombie wave 3 | until cleared | win | PvZ rules |
| win / lose | End screen | - | - | mod |

## Sheet: dash_items (60 Seconds files)
| id | item | gives | source asset |
|---|---|---|---|
| supply_sun | sun-ration | +25 starting sun | read from 60 Seconds folder: TBD |
| supply_seed | seed packet | unlocks a plant | read from 60 Seconds folder: TBD |
| family_member | family member | (v2: bonus) | read from 60 Seconds folder: TBD |

## Sheet: plants (PvZ files)
| id | name | cost | role | source asset |
|---|---|---|---|---|
| peashooter | Peashooter | 100 | shoots along lane | PvZ folder: TBD |
| sunflower | Sunflower | 50 | produces sun | PvZ folder: TBD |
| wallnut | Wall-nut | 50 | blocks zombies | PvZ folder: TBD |

## Sheet: zombies (PvZ files)
| id | name | health | speed | source asset |
|---|---|---|---|---|
| basic | Zombie | PvZ default | PvZ default | PvZ folder: TBD |

## Sheet: waves
| wave | zombies | count | start condition |
|---|---|---|---|
| 1 | basic | 3 | dash ends |
| 2 | basic | 6 | wave 1 cleared |
| 3 | basic | 10 | wave 2 cleared |

## Sheet: hooks (filled once host game is chosen)
| hook | purpose | status |
|---|---|---|
| host loader | which loader Melty installs for the host | TBD (game_info) |
| 60s_path_finder | locate 60 Seconds install via Steam libraries | TBD |
| pvz_path_finder | locate PvZ install via Steam libraries | TBD |
| missing_game_notice | in-game message when either game is absent | TBD |


## Preflight (open items)
- Host game not chosen.
- All "source asset: TBD" cells need the real files identified in the installed games.
- Dash item effects and wave numbers above are placeholders.
