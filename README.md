# Game2Vec
A GloVe Word2Vec Embeddings For Video Games
Based on Wikipedia and Steam, Trained using Gensim.

This repository includes Two Pairs of models each with a diffrenet vector size, each pair has one model using a reduced dictionary and one using the raw dictionary. While the reduced dictionary effectively removes many irrelevant tokens, it unfortunately also discards some interesting words. I still need to compile a better list of tokens to keep, but I haven’t gotten to that yet.

As you can see in the tables below, has some very cool and interesting matches that show the embeddings do have meaning and sometimes very accurate. but There are also examples that show it’s clearly not perfect and there is alot of room for improvment, it especially needs more accurate pruning.

I might work on this further in the future. For anyone interested in the dataset or the notebook, feel free to send me a message.

All words are lowercased spaces and - are converted to _.

Models in https://drive.google.com/drive/folders/1fwie0fR2MTqag8u5vQaCgjCxiQzGZUSS?usp=sharing

# 100 Pair

Raw Character Pairs Similarity (Raw Model)
| Pair           |   Similarity |
|----------------|--------------|
| mario - luigi  |     0.903821 |
| zelda - link   |     0.774103 |
| aerith - cloud |     0.694026 |
| aerith - zelda |     0.345711 |
| mario - cloud  |     0.229648 |

Raw Character Title Addition (Raw Model)
| Pair                   | Top 3 Similar                                                                          |
|------------------------|----------------------------------------------------------------------------------------|
| final_fantasy + aerith | final_fantasy_vii (0.8936), ffvii (0.8213), tifa (0.8194)                              |
| final_fantasy + cloud  | final_fantasy_vii (0.8416), square_enix_developed (0.7953), aerith (0.7889)            |
| final_fantasy + tidus  | final_fantasy_x (0.8601), kitase (0.8110), jecht (0.8045)                              |
| mario + cloud          | nintendo_switchmario (0.7328), hopemario (0.7274), thumbrightshigeru_miyamoto (0.7260) |


Genre Pairs Similarity
| Pair                |   Similarity |
|---------------------|--------------|
| rpg - fps           |     0.498238 |
| rpg - action        |     0.638042 |
| rpg - turn_based    |     0.696322 |
| action - turn_based |     0.526    |

Genre Addition
| Pair             | Top 3 Similar                                                                                |
|------------------|----------------------------------------------------------------------------------------------|
| rpg + fps        | fadeout_underground (0.8056), strife_1996 (0.8048), action_rpg (0.8033)                      |
| rpg + action     | wizardry_the_five_ordeals (0.8336), asterisk_2_next_now_a_days (0.8280), action_rpg (0.8265) |
| rpg + turn_based | turn_based_combat (0.8392), tactical_rpg (0.8345), quintaesencia (0.8344)                    |

Title-Genre Addition
| Pair                                | Top 3 Similar                                                                                                                  |
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| cyberpunk + the_witcher_3_wild_hunt | cd_projekt (0.7651), cyberpunk_2077 (0.7485), untitled_cyberpunk_2077_sequel (0.7462)                                          |
| medieval + cyberpunk_2077           | untitled_cyberpunk_2077_sequel (0.7589), marcin_przybyłowicz (0.7479), list_of_television_series_based_on_video_games (0.7428) |
| turn_based + dota                   | eonica_chess_battle (0.8171), hearthstone_battlegrounds (0.8106), bestiary_of_sigillum (0.7887)                                |

Title Pairs Similarity
| Pair                                        |   Similarity |
|---------------------------------------------|--------------|
| sekiro - bloodborne                         |     0.627428 |
| bloodborne - elden_ring                     |     0.758532 |
| elden_ring - sekiro                         |     0.624708 |
| cyberpunk_2077 - the_elder_scrolls_v_skyrim |     0.455388 |
| the_elder_scrolls_v_skyrim - elden_ring     |     0.49796  |
| elden_ring - cyberpunk_2077                 |     0.516961 |
| overcooked_all_you_can_eat - overcooked_2   |     0.807687 |
| sekiro - overcooked_2                       |     0.227203 |




# 300 Pair

Raw Character Pairs Similarity (Raw Model)
| Pair           |   Similarity |
|----------------|--------------|
| mario - luigi  |     0.826968 |
| zelda - link   |     0.680673 |
| aerith - cloud |     0.629857 |
| aerith - zelda |     0.171342 |
| mario - cloud  |     0.142214 |

Raw Character Title Addition (Raw Model)
| Pair                   | Top 3 Similar                                                                  |
|------------------------|--------------------------------------------------------------------------------|
| final_fantasy + aerith | final_fantasy_vii (0.7821), j_e_n_o_v_a (0.7508), chaos_final_fantasy (0.7082) |
| final_fantasy + cloud  | final_fantasy_vii (0.7478), chaos_final_fantasy (0.7198), j_e_n_o_v_a (0.7153) |
| final_fantasy + tidus  | final_fantasy_x (0.7839), auron (0.7327), jecht (0.7325)                       |
| mario + cloud          | nintendo_switchmario (0.6597), luigi (0.6493), doopliss (0.6483)               |

Genre Pairs Similarity
| Pair                |   Similarity |
|---------------------|--------------|
| rpg - fps           |     0.491896 |
| rpg - action        |     0.583057 |
| rpg - turn_based    |     0.59166  |
| action - turn_based |     0.427217 |

Genre Addition
| Pair             | Top 3 Similar                                                                     |
|------------------|-----------------------------------------------------------------------------------|
| rpg + fps        | action_adventure (0.7356), action_rpg (0.7332), action (0.7191)                   |
| rpg + action     | action_rpg (0.7220), untitled_crossing_record (0.7212), way_back_witness (0.7192) |
| rpg + turn_based | turn_based_combat (0.7873), jrpg (0.7540), golden_fall_2 (0.7536)                 |

Title-Genre Addition
| Pair                                | Top 3 Similar                                                                                                                      |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
| cyberpunk + the_witcher_3_wild_hunt | untitled_cyberpunk_2077_sequel (0.6994), cd_projekt (0.6876), list_of_television_series_based_on_video_games (0.6308)              |
| medieval + cyberpunk_2077           | the_witcher_monster_slayer (0.6580), untitled_cyberpunk_2077_sequel (0.6444), the_witcher_enhanced_edition_director's_cut (0.6433) |
| turn_based + dota                   | hearthstone_battlegrounds (0.6698), void_eclipse (0.6559), hartacon_tactics (0.6507)                                               |

Title Pairs Similarity
| Pair                                        |   Similarity |
|---------------------------------------------|--------------|
| sekiro - bloodborne                         |     0.448774 |
| bloodborne - elden_ring                     |     0.567204 |
| elden_ring - sekiro                         |     0.456767 |
| cyberpunk_2077 - the_elder_scrolls_v_skyrim |     0.266546 |
| the_elder_scrolls_v_skyrim - elden_ring     |     0.344332 |
| elden_ring - cyberpunk_2077                 |     0.313567 |
| overcooked_all_you_can_eat - overcooked_2   |     0.690596 |
| sekiro - overcooked_2                       |     0.141762 |
