# harry-item
Retarded harrys guide to item creation

items:
  ultra-item:
    id: DIAMOND_SWORD
    slot: 0
    name: '&bBlazefury'
    count: 1
    durability: 5
    lore:
      - '&7A god sword..'
      - '&7This is generations old!'
    commands:
      multi-click:
        - 'message: &eYou can send yourself custom messages!'
        - 'console: say You can even execute more than one command!'
        - 'player: say This is item slot 1'
        - 'say Hello world!'
      right-click:
        - 'console: gamemode 1 %player%'
        - 'message: &eYou have been set to creative mode.'
      left-click:
        - 'console: gamemode 3 %player%'
        - 'message: &eYou have been set to spectator mode.'
      multi-click-air:
        - 'message: &eThis will prevent commands from being executed when you click on blocks such as a sign.'
      right-click-air:
        - 'message: &eThis will prevent commands from being executed when you click on blocks such as a sign.'
      left-click-air:
        - 'message: &eThis will prevent commands from being executed when you click on blocks such as a sign.'
      inventory:
        - 'console: gamemode 2 %player%'
        - 'message: &eYou have been set to adventure mode.'
    enchantment: FIRE_ASPECT:3, DAMAGE_ALL:5, DAMAGE_UNDEAD:5, KNOCKBACK:8
    commands-type: interact, inventory
    commands-sequence: ALL, RANDOM
    commands-sound: BLOCK_NOTE_PLING
    commands-particle: FIREWORK:BLACK:RED:BURST:3
    commands-warmup: 5
    commands-cost: 25
    commands-cooldown: 5
    cooldown-message: '&7[&eItemJoin&7] &a[%item%&a] &cis on cooldown for &a%timeleft% &cseconds..'
    probability: 25
    use-cooldown: 10
    itemflags: inventory-modify, death-drops, unbreakable, disposable, count-lock, cancel-events, placement, hide-durability, hide-attributes, self-drops, first-join, CreativeBypass, AllowOpBypass
    triggers: join, respawn, world-change
    permission-node: 'itemjoin.ultra'
    enabled-regions: region1, region2
    enabled-worlds: world, world_nether, world_the_end
