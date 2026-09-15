# vanilla_raws_reference

> **Repository:** https://github.com/jaymorbin/vanilla_raws_reference
>
> ```
> git clone --depth 1 https://github.com/jaymorbin/vanilla_raws_reference.git
> ```
>
> **Companion repos:**
> - [df_data_reference](https://github.com/jaymorbin/df_data_reference) — path maps and structure dumps from a live game
> - [refinish_metal_tools](https://github.com/jaymorbin/refinish_metal_tools) — archived probe scripts, reference only
>
> A copy of this index also lives in the Refinish Metal project, where it is
> readable without cloning. See `REFERENCE_REPOS.md` there for the overview, and
> note that DFHack documentation is **not** in any repo.
> Both copies are generated; regenerate rather than hand-editing either.

Complete unmodified Dwarf Fortress vanilla raws, plus the vanilla sprite sheets. Mirrors DF's own mod folder layout, so the directory name tells you the object type before you open anything.

## How to use this

This is the authority for **what vanilla actually defines**: token spellings, existing material and reaction IDs, graphics tags, and name collisions to avoid when injecting new content.

```
grep -rln 'REACTION_CLASS:PITCH' vanilla_*/objects/
```

## Raws files (377 text files)

### `(root)/`

1 files, no OBJECT token

### `examples and notes/`

3 files, REACTION x1, ITEM x1, 8 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `reaction_instrument_example.txt` | REACTION | 4 | MAKE EXAMPLE DRUM BODY, MAKE EXAMPLE DRUM HEAD, MAKE EXAMPLE DRUM, MAKE EXAMPLE WIND |
| `item_instrument_example.txt` | ITEM | 4 | EXAMPLE DRUM BODY, EXAMPLE DRUM HEAD, EXAMPLE DRUM, EXAMPLE WIND |

### `interaction examples/`

9 files, INTERACTION x6, 13 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `interaction_secret.txt` | INTERACTION | 6 | EXAMPLE SECRET, EXAMPLE RAISE, EXAMPLE SUMMON, EXAMPLE UNDEAD LT RAISE |
| `interaction_disturbance.txt` | INTERACTION | 3 | EXAMPLE DISTURBANCE EFFECT, EXAMPLE CURSE, EXAMPLE D RAISE |
| `interaction_werebeast.txt` | INTERACTION | 2 | WEREBEAST_CURSE, WEREBEAST_BITE |
| `interaction_vampire.txt` | INTERACTION | 1 | VAMPIRE_CURSE |
| `interaction_region.txt` | INTERACTION | 1 | EXAMPLE DEAD ANIMATION IN EVIL REGIONS WITH MATERIAL CLOUDS AND RAIN |
| _...1 more_ | | | |

### `vanilla_bodies/`

1 files, no OBJECT token

### `vanilla_bodies/objects/`

4 files, BODY x2, BODY_DETAIL_PLAN x1, TISSUE_TEMPLATE x1, 293 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `body_default.txt` | BODY | 147 | BASIC_1PARTBODY, BASIC_1PARTBODY_THOUGHT, BASIC_1PARTBODY_FLYING_HEAD_FLAG_THOUGHT, BASIC_2PARTBODY |
| `body_rcp.txt` | BODY | 87 | RCP_BASIC_BODY, RCP_BASIC_BODY_STANCE, RCP_BASIC_BODY_STANCE_WITH_HEAD_FLAG, RCP_UPPER_BODY |
| `tissue_template_default.txt` | TISSUE_TEMPLATE | 38 | SKIN_TEMPLATE, FAT_TEMPLATE, MUSCLE_TEMPLATE, BONE_TEMPLATE |
| `b_detail_plan_default.txt` | BODY_DETAIL_PLAN | 21 | STANDARD_MATERIALS, CHITIN_MATERIALS, STANDARD_TISSUES, CHITIN_TISSUES |

### `vanilla_buildings/`

1 files, no OBJECT token

### `vanilla_buildings/objects/`

1 files, BUILDING x1

### `vanilla_buildings_graphics/`

1 files, no OBJECT token

### `vanilla_buildings_graphics/graphics/`

7 files, GRAPHICS x6, TILE_PAGE x1, 24 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_buildings.txt` | TILE_PAGE | 24 | LEVERS, ARCHERY_TARGETS, AXLES_GEARS, WINDMILL |

### `vanilla_creatures/`

1 files, no OBJECT token

### `vanilla_creatures/objects/`

35 files, CREATURE x31, TEXT_SET x3, CREATURE_VARIATION x1, 806 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `creature_birds_new.txt` | CREATURE | 84 | BIRD_CROW, CROW_MAN, GIANT_CROW, BIRD_RAVEN |
| `creature_large_tropical.txt` | CREATURE | 67 | ELEPHANT, ELEPHANT_MAN, GIANT_ELEPHANT, WARTHOG |
| `creature_temperate_new.txt` | CREATURE | 63 | WILD_BOAR, WILD_BOAR_MAN, GIANT_WILD_BOAR, COYOTE |
| `creature_tropical_new.txt` | CREATURE | 60 | MONGOOSE, MONGOOSE_MAN, GIANT_MONGOOSE, HYENA |
| `creature_large_temperate.txt` | CREATURE | 48 | BEAR_GRIZZLY, BEAR_GRIZZLY_MAN, GIANT_BEAR_GRIZZLY, BEAR_BLACK |
| `creature_bug_slug_new.txt` | CREATURE | 43 | DAMSELFLY, DAMSELFLY_MAN, GIANT_DAMSELFLY, MOTH |
| `creature_large_ocean.txt` | CREATURE | 40 | WALRUS, WALRUS_MAN, GIANT_WALRUS, FISH_LAMPREY_SEA |
| `c_variation_default.txt` | CREATURE_VARIATION | 36 | ANIMAL_PERSON, ANIMAL_PERSON_LEGLESS, PUNCH_ATTACK, KICK_ATTACK |
| _...27 more_ | | | |

### `vanilla_creatures_extinct/`

1 files, no OBJECT token

### `vanilla_creatures_extinct/objects/`

10 files, CREATURE x10, 200 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `creature_cretaceous.txt` | CREATURE | 62 | CRETACEOUS_AMMONITE, CRETACEOUS_AMMONITE_MAN, CRETACEOUS_ARCHELON, CRETACEOUS_ARCHELON_MAN |
| `creature_cenozoic.txt` | CREATURE | 40 | CENOZOIC_DEINOTHERIUM, CENOZOIC_DEINOTHERIUM_MAN, CENOZOIC_SMILODON, CENOZOIC_SMILODON_MAN |
| `creature_jurassic.txt` | CREATURE | 36 | JURASSIC_ICHTHYOSAURUS, JURASSIC_ICHTHYOSAURUS_MAN, JURASSIC_TORVOSAURUS, JURASSIC_TORVOSAURUS_MAN |
| `creature_permian.txt` | CREATURE | 14 | PERMIAN_DIPLOCAULUS, PERMIAN_DIPLOCAULUS_MAN, PERMIAN_ERYOPS, PERMIAN_ERYOPS_MAN |
| `creature_cambrian.txt` | CREATURE | 12 | CAMBRIAN_HALLUCIGENIA, CAMBRIAN_HALLUCIGENIA_MAN, CAMBRIAN_HAIKOUICHTHYS, CAMBRIAN_HAIKOUICHTHYS_MAN |
| `creature_devonian.txt` | CREATURE | 12 | DEVONIAN_DUNKLEOSTEUS, DEVONIAN_DUNKLEOSTEUS_MAN, DEVONIAN_TIKTAALIK, DEVONIAN_TIKTAALIK_MAN |
| `creature_triassic.txt` | CREATURE | 12 | TRIASSIC_GERROTHORAX, TRIASSIC_GERROTHORAX_MAN, TRIASSIC_EORAPTOR, TRIASSIC_EORAPTOR_MAN |
| `creature_carboniferous.txt` | CREATURE | 8 | CARBONIFEROUS_OESTOCEPHALUS, CARBONIFEROUS_OESTOCEPHALUS_MAN, CARBONIFEROUS_TULLIMONSTRUM, CARBONIFEROUS_TULLIMONSTRUM_MAN |
| _...2 more_ | | | |

### `vanilla_creatures_extinct_graphics/`

1 files, no OBJECT token

### `vanilla_creatures_extinct_graphics/graphics/`

62 files, GRAPHICS x60, TILE_PAGE x2, 60 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_creatures.txt` | TILE_PAGE | 40 | CREATURES_CAMBRIAN, STATUES_CREATURES_CAMBRIAN, CREATURES_CARBONIFEROUS, STATUES_CREATURES_CARBONIFEROUS |
| `tile_page_portraits.txt` | TILE_PAGE | 20 | PORTRAIT_CREATURES_CAMBRIAN, PORTRAIT_CREATURES_CARBONIFEROUS, PORTRAIT_CREATURES_CENOZOIC, PORTRAIT_CREATURES_CRETACEOUS |
| _...54 more_ | | | |

### `vanilla_creatures_graphics/`

1 files, no OBJECT token

### `vanilla_creatures_graphics/graphics/`

60 files, GRAPHICS x57, TILE_PAGE x3, 230 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_portraits.txt` | TILE_PAGE | 127 | PORTRAIT_DWARF_BODY, PORTRAIT_DWARF_HAIR, PORTRAIT_DWARF_CLOTHING_UNDER, PORTRAIT_DWARF_CLOTHING_CAP |
| `tile_page_creatures.txt` | TILE_PAGE | 95 | BODYPARTS, BONE_PILE, GUTS, CREATURES_ANIMAL_PEOPLE |
| `tile_page_layered_corpses.txt` | TILE_PAGE | 8 | DWARF_BODY_CORPSE, DWARF_HAIR_CORPSE, HUMAN_BODY_CORPSE, HUMAN_HAIR_CORPSE |
| _...52 more_ | | | |

### `vanilla_descriptors/`

1 files, no OBJECT token

### `vanilla_descriptors/objects/`

5 files, DESCRIPTOR_PATTERN x3, DESCRIPTOR_COLOR x1, DESCRIPTOR_SHAPE x1, 136 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `descriptor_color_standard.txt` | DESCRIPTOR_COLOR | 136 | AMBER, AMETHYST, AQUA, AQUAMARINE |

### `vanilla_descriptors_graphics/`

1 files, no OBJECT token

### `vanilla_descriptors_graphics/graphics/`

3 files, PALETTE x1, TILE_PAGE x1, GRAPHICS x1, 5 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `palette_default.txt` | PALETTE | 3 | DEFAULT, NEX_BODY, BEASTS |
| `tile_page_descriptors.txt` | TILE_PAGE | 2 | GEMS, SMALLGEMS |

### `vanilla_entities/`

1 files, no OBJECT token

### `vanilla_entities/objects/`

1 files, ENTITY x1, 6 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `entity_default.txt` | ENTITY | 6 | MOUNTAIN, FOREST, PLAINS, EVIL |

### `vanilla_environment/`

1 files, no OBJECT token

### `vanilla_environment/graphics/`

6 files, GRAPHICS x5, TILE_PAGE x1, 88 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_environment.txt` | TILE_PAGE | 88 | FLOWS, FLOWS2, FLOWS3, FLOWS4 |

### `vanilla_interactions/`

1 files, no OBJECT token

### `vanilla_interactions/objects/`

1 files, INTERACTION x1, 5 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `interaction_standard.txt` | INTERACTION | 5 | CLEANING, BP_BUMP, PET_ANIMAL, MATERIAL_EMISSION |

### `vanilla_interactions_graphics/`

1 files, no OBJECT token

### `vanilla_interactions_graphics/graphics/`

2 files, TILE_PAGE x1, GRAPHICS x1, 1 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_interactions.txt` | TILE_PAGE | 1 | INTERACTION_LIST_ICONS |

### `vanilla_interface/`

1 files, no OBJECT token

### `vanilla_interface/graphics/`

10 files, GRAPHICS x9, TILE_PAGE x1, 66 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_interface.txt` | TILE_PAGE | 66 | INTERFACE_BITS_SHARED, ANNOUNCEMENT_ALERTS, UNIT_STATUS, BUILDING_ICONS |
| _...2 more_ | | | |

### `vanilla_items/`

1 files, no OBJECT token

### `vanilla_items/objects/`

13 files, ITEM x13, 112 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `item_tool.txt` | ITEM | 30 | ITEM_TOOL_CAULDRON, ITEM_TOOL_LADLE, ITEM_TOOL_BOWL, ITEM_TOOL_MORTAR |
| `item_weapon.txt` | ITEM | 25 | ITEM_WEAPON_WHIP, ITEM_WEAPON_AXE_BATTLE, ITEM_WEAPON_HAMMER_WAR, ITEM_WEAPON_SWORD_SHORT |
| `item_armor.txt` | ITEM | 12 | ITEM_ARMOR_BREASTPLATE, ITEM_ARMOR_MAIL_SHIRT, ITEM_ARMOR_LEATHER, ITEM_ARMOR_COAT |
| `item_pants.txt` | ITEM | 9 | ITEM_PANTS_PANTS, ITEM_PANTS_GREAVES, ITEM_PANTS_LEGGINGS, ITEM_PANTS_LOINCLOTH |
| `item_helm.txt` | ITEM | 8 | ITEM_HELM_HELM, ITEM_HELM_CAP, ITEM_HELM_HOOD, ITEM_HELM_TURBAN |
| `item_shoes.txt` | ITEM | 6 | ITEM_SHOES_SHOES, ITEM_SHOES_BOOTS, ITEM_SHOES_BOOTS_LOW, ITEM_SHOES_SANDAL |
| `item_toy.txt` | ITEM | 5 | ITEM_TOY_PUZZLEBOX, ITEM_TOY_BOAT, ITEM_TOY_HAMMER, ITEM_TOY_AXE |
| `item_trapcomp.txt` | ITEM | 5 | ITEM_TRAPCOMP_GIANTAXEBLADE, ITEM_TRAPCOMP_ENORMOUSCORKSCREW, ITEM_TRAPCOMP_SPIKEDBALL, ITEM_TRAPCOMP_LARGESERRATEDDISC |
| _...5 more_ | | | |

### `vanilla_items_graphics/`

1 files, no OBJECT token

### `vanilla_items_graphics/graphics/`

5 files, GRAPHICS x4, TILE_PAGE x1, 39 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_items.txt` | TILE_PAGE | 39 | ITEM_CRAFTS, ITEM_FOOD, ITEM_TOY, ITEM_TRAPCOMP |

### `vanilla_languages/`

1 files, no OBJECT token

### `vanilla_languages/objects/`

6 files, LANGUAGE x6

### `vanilla_materials/`

1 files, no OBJECT token

### `vanilla_materials/objects/`

7 files, INORGANIC x6, MATERIAL_TEMPLATE x1, 335 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `inorganic_stone_gem.txt` | INORGANIC | 127 | ONYX, MORION, SCHORL, LACE AGATE |
| `material_template_default.txt` | MATERIAL_TEMPLATE | 70 | STONE_TEMPLATE, METAL_TEMPLATE, WOOD_TEMPLATE, SKIN_TEMPLATE |
| `inorganic_stone_mineral.txt` | INORGANIC | 58 | HEMATITE, LIMONITE, GARNIERITE, NATIVE_GOLD |
| `inorganic_metal.txt` | INORGANIC | 26 | IRON, GOLD, SILVER, COPPER |
| `inorganic_stone_layer.txt` | INORGANIC | 25 | SANDSTONE, SILTSTONE, MUDSTONE, SHALE |
| `inorganic_stone_soil.txt` | INORGANIC | 21 | CLAY, SILTY_CLAY, SANDY_CLAY, CLAY_LOAM |
| `inorganic_other.txt` | INORGANIC | 8 | PLASTER, CERAMIC_EARTHENWARE, CERAMIC_STONEWARE, CERAMIC_PORCELAIN |

### `vanilla_music/`

1 files, no OBJECT token

### `vanilla_music/objects/`

2 files, MUSIC x1, SOUND x1, 47 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `music_standard.txt` | MUSIC | 29 | TRACK_01, TRACK_02, TRACK_03, TRACK_04 |
| `sound_standard.txt` | SOUND | 18 | ADAMANTINE, AMBUSH, ARTIFACT_CREATED, BABY_BORN |

### `vanilla_plants/`

1 files, no OBJECT token

### `vanilla_plants/objects/`

5 files, PLANT x5, 225 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `plant_garden.txt` | PLANT | 57 | ARTICHOKE, ASPARAGUS, BAMBARA_GROUNDNUT, STRING_BEAN |
| `plant_standard.txt` | PLANT | 52 | MUSHROOM_HELMET_PLUMP, GRASS_TAIL_PIG, GRASS_WHEAT_CAVE, POD_SWEET |
| `plant_new_trees.txt` | PLANT | 41 | ABACA, BANANA, CARAMBOLA, CASHEW |
| `plant_grasses.txt` | PLANT | 41 | MEADOW-GRASS, HAIR GRASS, BENTGRASS, RYEGRASS |
| `plant_crops.txt` | PLANT | 34 | SINGLE-GRAIN_WHEAT, TWO-GRAIN_WHEAT, SOFT_WHEAT, HARD_WHEAT |

### `vanilla_plants_graphics/`

1 files, no OBJECT token

### `vanilla_plants_graphics/graphics/`

7 files, GRAPHICS x6, TILE_PAGE x1, 36 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_plants.txt` | TILE_PAGE | 36 | GRASS, GRASS_FLOWERS, GRASS_OTHER, CAVERN_GRASS |

### `vanilla_procedural/`

1 files, no OBJECT token

### `vanilla_procedural/scripts/`

1 files, no OBJECT token

### `vanilla_procedural/scripts/generators/`

8 files, no OBJECT token

### `vanilla_procedural/scripts/generators/creatures/`

2 files, no OBJECT token

### `vanilla_procedural/scripts/generators/interactions/`

6 files, no OBJECT token

### `vanilla_reactions/`

1 files, no OBJECT token

### `vanilla_reactions/objects/`

4 files, REACTION x4, 159 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `reaction_dyes.txt` | REACTION | 68 | ACACIA_BARK_DYE, ALDER_BARK_DYE, ALDER_CONE_DYE, ALMOND_SHELL_DYE |
| `reaction_other.txt` | REACTION | 46 | TAN_A_HIDE, RENDER_FAT, MAKE_SOAP_FROM_TALLOW, MAKE_SOAP_FROM_OIL |
| `reaction_smelter.txt` | REACTION | 23 | BITUMINOUS_COAL_TO_COKE, LIGNITE_TO_COKE, BRASS_MAKING, BRASS_MAKING2 |
| `reaction_adv_carpenter.txt` | REACTION | 22 | MAKE WOODEN CHAIR, MAKE WOODEN TABLE, MAKE WOODEN BED, MAKE WOODEN CHEST |

### `vanilla_text/`

1 files, no OBJECT token

### `vanilla_text/objects/`

64 files, TEXT_SET x64, 64 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `text_same_site_ab_specific_hf_seeker.txt` | TEXT_SET | 1 | SAME_SITE_AB_SPECIFIC_HF_SEEKER |
| `text_justification_reminder.txt` | TEXT_SET | 1 | JUSTIFICATION_REMINDER |
| `text_mercenary_profession.txt` | TEXT_SET | 1 | MERCENARY_PROFESSION |
| `text_unknown_hf_seeker.txt` | TEXT_SET | 1 | UNKNOWN_HF_SEEKER |
| `text_greet_worship.txt` | TEXT_SET | 1 | GREET_WORSHIP |
| `text_family_relationship_additional_dead.txt` | TEXT_SET | 1 | FAMILY_RELATIONSHIP_ADDITIONAL_DEAD |
| `text_temple_become_member.txt` | TEXT_SET | 1 | TEMPLE_BECOME_MEMBER |
| `text_thief_profession.txt` | TEXT_SET | 1 | THIEF_PROFESSION |
| _...56 more_ | | | |

### `vanilla_world_map/`

1 files, no OBJECT token

### `vanilla_world_map/graphics/`

2 files, TILE_PAGE x1, GRAPHICS x1, 20 definitions total

| File | Object | Defs | Examples |
|---|---|---|---|
| `tile_page_world_map.txt` | TILE_PAGE | 20 | WORLD_MAP_TILES, WORLD_MAP_MOUNTAINS, WORLD_MAP_FORESTS, WORLD_MAP_EDGE_SHAPES |

## Sprite sheets (585 images across 20 directories)

| Directory | Images | Size |
|---|---|---|
| `vanilla_creatures_graphics/graphics/images/` | 75 | 4063K |
| `vanilla_environment/graphics/images/` | 89 | 2016K |
| `vanilla_creatures_graphics/graphics/images/portraits/` | 137 | 1672K |
| `vanilla_plants_graphics/graphics/images/` | 36 | 1288K |
| `vanilla_world_map/graphics/images/` | 20 | 1216K |
| `vanilla_buildings_graphics/graphics/images/` | 24 | 899K |
| `vanilla_creatures_extinct_graphics/graphics/images/` | 20 | 899K |
| `vanilla_interface/graphics/images/` | 66 | 553K |
| `vanilla_creatures_extinct_graphics/graphics/images/portraits/` | 20 | 513K |
| `vanilla_items_graphics/graphics/images/` | 38 | 446K |
| `vanilla_creatures_graphics/graphics/images/dwarf/` | 8 | 108K |
| `vanilla_creatures_extinct_graphics/graphics/images/statues/` | 20 | 108K |
| `vanilla_creatures_graphics/graphics/images/human/` | 6 | 51K |
| `vanilla_creatures_graphics/graphics/images/elf/` | 6 | 48K |
| `vanilla_creatures_graphics/graphics/images/goblin/` | 4 | 38K |
| `vanilla_descriptors_graphics/graphics/images/` | 5 | 37K |
| `vanilla_creatures_graphics/graphics/images/ogres/` | 4 | 36K |
| `vanilla_creatures_graphics/graphics/images/kobold/` | 4 | 36K |
| `vanilla_creatures_graphics/graphics/images/troll/` | 2 | 8K |
| `vanilla_interactions_graphics/graphics/images/` | 1 | 2K |

## Notes

- `readme.txt` at the root is **Bay 12's public-domain waiver** that shipped with the raws, not a description of this repo. GitHub renders it as the landing page.
- Images remain under copyright per that notice; the text raws are public domain.