Back to [world database](mangosdb_struct) list of tables.

The \`spell\_bonus\_data\` table
--------------------------------

Table used for storing custom damage/healing bonus coefficients.

### Structure

| **Field**                                       | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
|-------------------------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| [entry](Spell_bonus_data#entry)                 | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [direct\_bonus](Spell_bonus_data#direct_bonus)  | float        | signed         |         | NO       | 0           |           |             |
| [dot\_bonus](Spell_bonus_data#dot_bonus)        | float        | signed         |         | NO       | 0           |           |             |
| [ap\_bonus](Spell_bonus_data#ap_bonus)          | float        | signed         |         | NO       | 0           |           |             |
| [ap\_dot\_bonus](Spell_bonus_data#ap_dot_bonus) | float        | signed         |         | NO       | 0           |           |             |
| [comments](Spell_bonus_data#comments)           | varchar(255) | signed         |         | YES      | NULL        |           |             |

### Description of the fields

#### entry

Spell ID. See [Spell.dbc.](Spell.dbc).

#### direct\_bonus

Direct spell power damage.<br>
If < 0<br>
Calculate default spell power coefficient.<br>
If = 0<br>
Don't apply any spell power coefficient. (Don't scale damage with spellpower)<br>
If > 0<br>
Use this as new spell power coefficient.

#### dot\_bonus

Spell damage over time.<br>
If < 0<br>
Calculate default spell power coefficient.<br>
If = 0<br>
Don't apply any spell power coefficient. (Don't scale damage with spellpower)<br>
If > 0<br>
Use this as new spell power coefficient.

#### ap\_bonus

Direct Melee/Ranged damage.<br>
If < 0<br>
Calculate default attack power coefficient.<br>
If = 0<br>
Don't apply any attack power coefficient. (Don't scale damage with attack power)<br>
If > 0<br>
Use this as new attack power coefficient.

#### ap\_dot\_bonus

Melee/Ranged damage over time.<br>
If < 0<br>
Calculate default attack power coefficient.<br>
If = 0<br>
Don't apply any attack power coefficient. (Don't scale damage with attack power)<br>
If > 0<br>
Use this as new attack power coefficient.

#### comments

Comment as why it has such values and name of the spell.
