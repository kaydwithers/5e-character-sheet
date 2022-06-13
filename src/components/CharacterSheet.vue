<script setup lang="ts">
import type { CharacterInterface } from "@/interfaces/characterInterface";

defineProps<{
  character: CharacterInterface;
}>();
</script>

<template>
  <div class="page">
    <div class="layout layout--small mb2">
      <!-- Character -->
      <div class="layout__item flex-1">
        <div class="bg-grey">
          <div class="bg-white">
            <h5>{{ character.name }}</h5>
            <small class="mb0 tt-u">Character name</small>
          </div>
        </div>
      </div>

      <div class="layout__item">
        <div class="bg-grey">
          <div class="bg-white">
            <h5>{{ character.occupation }} Level {{ character.level }}</h5>
            <small class="mb0 tt-u">Class &amp; Level</small>
          </div>
        </div>
      </div>

      <div class="layout__item">
        <div class="bg-grey">
          <div class="bg-white">
            <h5>{{ character.race }}</h5>
            <small class="mb0 tt-u">Race</small>
          </div>
        </div>
      </div>

      <div class="layout__item">
        <div class="bg-grey">
          <div class="bg-white">
            <h5>{{ character.alignment }}</h5>
            <small class="mb0 tt-u">Alignment</small>
          </div>
        </div>
      </div>
    </div>

    <div class="layout layout--small">
      <!-- Stats -->
      <div class="layout__item one-third mb2">
        <div class="layout mb2">
          <div class="layout__item one-third">
            <div class="bg-grey">
              <div class="bg-white pv2 ph0 ta-c mb2">
                <small class="tt-u mb2">Strength</small>
                <h5>+3</h5>
                <small>16</small>
              </div>

              <div class="bg-white pv2 ph0 ta-c mb2">
                <small class="tt-u mb2">Dexterity</small>
                <h5>+4</h5>
                <small>18</small>
              </div>

              <div class="bg-white pv2 ph0 ta-c mb2">
                <small class="tt-u mb2">Constitution</small>
                <h5>+3</h5>
                <small>16</small>
              </div>

              <div class="bg-white pv2 ph0 ta-c mb2">
                <small class="tt-u mb2">Intelligence</small>
                <h5>+0</h5>
                <small>11</small>
              </div>

              <div class="bg-white pv2 ph0 ta-c mb2">
                <small class="tt-u mb2">Wisdom</small>
                <h5>-1</h5>
                <small>8</small>
              </div>

              <div class="bg-white pv2 ph0 ta-c">
                <small class="tt-u mb2">Charisma</small>
                <h5>+2</h5>
                <small>11</small>
              </div>
            </div>
          </div>

          <!-- Skills -->
          <div class="layout__item two-thirds">
            <div class="bg-white mb2">
              <p class="tt-u mb0">
                <span class="pr1">+2</span> Proficiency Bonus
              </p>
            </div>
            <div class="bg-white mb2">
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">+3</span> Strength
              </p>
              <p class="mb1">
                <span class="circle">●</span
                ><span class="pr1 td-u">+4</span> Dexterity
              </p>
              <p class="mb1">
                <span class="circle">●</span
                ><span class="pr1 td-u">+3</span> Constitution
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Intelligence
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">-1</span> Wisdom
              </p>
              <p class="">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Charisma
              </p>
              <small class="tt-u ta-c">Saving Throws</small>
            </div>
            <div class="bg-white">
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">+4</span> Acrobatics
                <span class="grey">(Dex)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Animal Handling
                <span class="grey">(Wis)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Arcana
                <span class="grey">(Int)</span>
              </p>
              <p class="mb1">
                <span class="circle">●</span
                ><span class="pr1 td-u">+5</span> Athletics
                <span class="grey">(Str)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Deception
                <span class="grey">(Cha)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> History
                <span class="grey">(Int)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">-1</span> Insight
                <span class="grey">(Wis)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Intimidation
                <span class="grey">(Cha)</span>
              </p>
              <p class="mb1">
                <span class="circle">●</span
                ><span class="pr1 td-u">+2</span> Investigation
                <span class="grey">(Int)</span>
              </p>
              <p class="mb1">
                <span class="circle">●</span
                ><span class="pr1 td-u">+1</span> Medicine
                <span class="grey">(Wis)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Nature
                <span class="grey">(Int)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">-1</span> Perception
                <span class="grey">(Wis)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Performance
                <span class="grey">(Cha)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Persuasion
                <span class="grey">(Cha)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">0</span> Religion
                <span class="grey">(Int)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">+4</span> Sleight of Hand
                <span class="grey">(Dex)</span>
              </p>
              <p class="mb1">
                <span class="circle">○</span
                ><span class="pr1 td-u">+4</span> Stealth
                <span class="grey">(Dex)</span>
              </p>
              <p class="">
                <span class="circle">●</span
                ><span class="pr1 td-u">+1</span> Survival
                <span class="grey">(Wis)</span>
              </p>
              <small class="mb0 tt-u ta-c">Skills</small>
            </div>
          </div>
        </div>

        <div class="layout">
          <!-- Proficiencies -->
          <div class="layout__item one-whole">
            <div class="bg-white">
              <p>
                <b>Armour proficiencies: </b>Light Armour, Medium Armour, Heavy
                Armour, Shields
              </p>
              <p>
                <b>Weapon proficiencies: </b>Simple Weapons, Martial Weapons
              </p>
              <p><b>Languages: </b>Common, Goblin, Dwarven</p>
              <p>
                <b>Nimble Escape:</b>. Goblins know when to run when things get
                heated. When you are the target of an opportunity attack, you
                may use your reaction to impose disadvantage on that attack.
              </p>
              <p>
                <b>Darkvision:</b> You have superior vision in dark and dim
                conditions. You can see in dim light within 60 feet of you as if
                it were bright light, and in darkness as if it were dim light.
                You can’t discern color in darkness, only shades of gray.
              </p>

              <small class="mb0 tt-u ta-c">Proficiencies &amp; Languages</small>
            </div>
          </div>
        </div>
      </div>

      <div class="layout__item one-third">
        <div class="bg-grey mb2">
          <div class="layout pb2">
            <!-- Armour Class -->
            <section class="layout__item one-third ta-c">
              <div class="bg-white">
                <h5>16</h5>
                <small class="mb0 tt-u">AC</small>
              </div>
            </section>

            <!-- Initiative -->
            <section class="layout__item one-third ta-c">
              <div class="bg-white">
                <h5>4</h5>
                <small class="mb0 tt-u">Initiative</small>
              </div>
            </section>

            <!-- Speed -->
            <section class="layout__item one-third ta-c">
              <div class="bg-white">
                <h5>30 feet</h5>
                <small class="mb0 tt-u">Speed</small>
              </div>
            </section>
          </div>

          <!-- Hit points -->
          <div class="pb2">
            <div class="bg-white">
              <p class="mb5 pb3">
                Hit point maximum <span class="td-u">47</span>
              </p>
              <small class="mb0 tt-u ta-c">Current hit points</small>
            </div>
          </div>

          <!-- Temporary hit points -->
          <div class="pb2">
            <div class="bg-white">
              <p class="pb2"></p>
              <small class="mb0 tt-u ta-c">Temporary hit points</small>
            </div>
          </div>

          <div class="layout display-flex">
            <!-- Hit dice -->
            <div class="layout__item one-half ta-c">
              <div class="bg-white">
                <h5>17</h5>
                <small class="mb0 tt-u">Hit dice</small>
              </div>
            </div>

            <!-- Death saves -->
            <div class="layout__item one-half ta-c">
              <div class="bg-white ta-r">
                <p class="tt-u mb0">
                  <small
                    >Successes <span class="circle pl1">○</span
                    ><span class="circle">○</span
                    ><span class="circle pr0">○</span></small
                  >
                </p>
                <p class="tt-u">
                  <small
                    >Failures <span class="circle pl1">○</span
                    ><span class="circle">○</span
                    ><span class="circle pr0">○</span></small
                  >
                </p>
                <small class="mb0 tt-u ta-c">Death saves</small>
              </div>
            </div>
          </div>
        </div>

        <div class="layout">
          <div class="layout__item pb2">
            <div class="bg-white">
              <img
                class="one-whole"
                src="http://res.cloudinary.com/dvjpaoffl/image/upload/v1486636435/winston_brf7my.jpg"
                alt="winston"
              />
            </div>
          </div>
        </div>

        <div class="layout">
          <!-- Attacks -->
          <section class="layout__item one-whole mb2">
            <div class="bg-white">
              <!-- Warhammer -->
              <div class="layout layout--tiny mb2">
                <div class="layout__item two-fifths">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">Warhammer</p>
                  </div>
                </div>

                <div class="layout__item one-fifth">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">+5</p>
                  </div>
                </div>

                <div class="layout__item two-fifths">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">1d8+3 bludgeon</p>
                  </div>
                </div>
              </div>

              <!-- Javelin -->
              <div class="layout layout--tiny mb2">
                <div class="layout__item two-fifths">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">Javelin</p>
                  </div>
                </div>

                <div class="layout__item one-fifth">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">+5</p>
                  </div>
                </div>

                <div class="layout__item two-fifths">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">1d6+3 piercing</p>
                  </div>
                </div>
              </div>

              <!-- Spell -->
              <div class="layout layout--tiny mb2">
                <div class="layout__item two-fifths">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">Spell Attack</p>
                  </div>
                </div>

                <div class="layout__item one-fifth">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">+2</p>
                  </div>
                </div>

                <div class="layout__item two-fifths">
                  <div class="bg grey-light ta-c p1">
                    <p class="mb0 black">Spell DC: 10</p>
                  </div>
                </div>
              </div>

              <p class="">
                You can throw a javelin 30 feet, or up to 120 feet with
                disadvantage on the attack roll.
              </p>

              <small class="mb0 tt-u ta-c">Attacks &amp; Spellcasting</small>
            </div>
          </section>
        </div>

        <div class="layout">
          <!-- Equipment -->
          <section class="layout__item one-whole">
            <div class="bg-white">
              <p class="mb0">Chain mail</p>
              <p class="mb0">Warhammer</p>
              <p class="mb0">Martial weapon</p>
              <p class="mb0">Javelin (5)</p>
              <p class="mb0">Priests pack</p>
              <p class="mb0">Holy symbol</p>
              <p class="mb0">Monster hunter's pack</p>
              <p class="">Important trinket</p>
              <small class="mb0 tt-u ta-c">Equipment</small>
            </div>
          </section>
        </div>
      </div>

      <div class="layout__item one-third">
        <!-- Personality -->
        <div class="bg-grey mb2">
          <div class="bg-white mb2">
            <p>I love animals.</p>
            <small class="mb0 tt-u ta-c">Personality Traits</small>
          </div>

          <div class="bg-white mb2">
            <p>
              Always wanted to ride into battle on a worg. I must avenge my
              buddy Hugs.
            </p>
            <small class="mb0 tt-u ta-c">Ideals</small>
          </div>

          <div class="bg-white mb2">
            <p>My dragon onesie makes me feel safe at night.</p>
            <small class="mb0 tt-u ta-c">Bonds</small>
          </div>

          <div class="bg-white">
            <p>Often do more harm than good. But I mean well.</p>
            <small class="mb0 tt-u ta-c">Flaws</small>
          </div>
        </div>

        <!-- Features -->
        <div class="bg-white">
          <p class="">
            <b>Second Wind:</b> You have a limited well of stamina you can draw
            on to protect yourself from harm. You can use a bonus action to
            regain hit points equal to 1d10+ your fighter level.
          </p>
          <p class="">
            <b>Goblin Features:</b> Within 60 feet of you, treat dim light as
            bright, darkness as dim light.
          </p>
          <p class="">
            You can deal your level extra damage with a spell or attack to a
            creature larger than you. (1/rest)
          </p>
          <p class="">As a bonus action, you can hide or disengage.</p>
          <p class="">
            <b>Haunted One Features:</b> Commoners will do what they can to help
            you.
          </p>
          <p class="">
            <b>Paladin Features:</b> As an action, detect the location of any
            celestial, fiend or undead and any consecrated or desecrated place
            or object within 60 feet (1 + Cha mod per day)
          </p>
          <p class="">
            Gain a reservoir or healing power (20hp), and as an action, you can
            heal a creature you touch by draining that power. You can also cure
            one poison or disease from the creature by sacrificing 5hp from the
            reservoir.
          </p>
          <p class="">
            <b>Fighting Style:</b> Protection: As a reaction, use your shield to
            impose disadvantage when an adjacent enemy attacks someone else.
          </p>
          <p class="">
            You can sacrific a spell slot to deal (1 + spell level)d8 radiant
            damage plus 1d8 extra damage vs undead/fiends, when you hit with a
            melee weapon attack.
          </p>
          <p class="">Gain immunity to disease.</p>
          <p class=""><b>Paladin Archetype:</b> Vengeance</p>
          <p class="">Abjure Enemy (see rules)</p>
          <p class="">Vow of Enmity (see rules)</p>
          <small class="mb0 tt-u ta-c">Features &amp; Traits</small>
        </div>
      </div>
    </div>
  </div>
</template>
