---
layout: default
title: Making Fun Cards
zeu: 1
---

"Making Fun Cards" is, to some extent, the entire purpose of custom Magic design. Its a problem that will never be solved completely, and this guide can’t instruct you on how to be perfect at it. Regardless, this section will give you some wider principles to think about when trying to make fun cards.

### Elegance in Play

**Cards should be about what they are about**. Whenever you create a card it should have a clear purpose for what fun it is supposed to create, and should lack elements that distract from or go against that purpose.

In elegant designs, no elements of the design are fighting against its main purpose. A classic category of cards that fight against themselves are cards that both encourage and discourage the same action. For example, a card that rewards constantly attacking but also rewards always keeping up blockers would be inelegant since the player can’t really do both of those things at the same time.

**Extraneous elements are inelegant**. You should avoid elements of a design that appear extraneous to players. This means players think that one part has nothing to do with how the rest of the card is played. More importantly, you should avoid elements that actually are extraneous. This means elements that are never utilized by players or never become relevant when playing with a card. Occasionally players will think a design has an extraneous element, but it's actually relevant in play often enough to justify being included.

### Interesting Decisions
<div class="row">
    <div class="col-sm-8">
        <p>Many <b>fun cards provide meaningful decisions</b> to the player. If a card has the potential for decision making, try to evaluate in which situations players will make one side of a choice and in which situations players will make the other choice. This will help you to see if the choice is actually meaningful. You might find that one side of the choice is correct almost all of the time. </p>
        <p>Take this custom card selection spell, for example.</p>
        <p>In the vast majority of situations, the first mode is better than the second mode. This card offers the player a <b>false choice</b>. Anyone who tries to min-max their use of the card will be frustrated, since its both difficult and uninteresting to try determining when the second mode is better than the first mode, and any player who naively tries to determine through experimentation will be met with subpar results. Players in the Spike psychographic especially hate cards that offer false choices like this.</p>
        <p>Magic naturally provides decisions to the player. Its possible to make designs that strip these decisions from the game by giving the player a path towards victory that is too clear. This can lead to un-satisfying gameplay, so be aware of it.</p>
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/false-choice-card-selection.png">
    </div>
</div>

### Gameplay Loops

A gameplay loop is a **series of actions that a player will find fun to perform** whenever they use a card. Many cards create their own gameplay loops, because of the effects they do or the way they interact with other actions (drawing cards, attacking with creatures, etc.)

You can focus on creating gameplay loops on many permanent cards. Planeswalkers are primarily focused on creating gameplay loops. Artifacts and enchantments are also often geared towards it.
<div class="row">
    <div class="col-sm-6">
<img class="img-fluid" src="{{ site.baseurl }}/css/imgs/trading-post.png">
    </div>
    <div class="col-sm-6">
<img class="img-fluid" src="{{ site.baseurl }}/css/imgs/ajani-valiant-protector.png">
    </div>
</div>
<br>
Trading Post and Ajani, Valiant protector are both examples of cards with strong, obvious gameplay loops.

Don’t confuse "gameplay loops" with continuous recurring a single card, which is also referred to as “looping”. Also don’t confuse “gameplay loops” with infinite or quasi-infinite combos.

### Rules of Thumb: Complexity

These are some of the easiest ways to avoid frustrating complexity.

* Make sure that anything that needs to be remembered for more than a turn cycle (one turn each for you and your opponent(s)) is marked in some way.
    * Counters
        * +1/+1 counters for marking a change, like with renown or monstrous.
        * Special named counters for unusual lasting effects of cards.
    * Card exiled underneath another.
* Avoid trigger times that are harder to remember.
    * Upkeep and end step are harder to remember, and should be kept out of commons.
    * Enter the battlefield and attack triggers are comparatively easier.

### Common Unintuitive Templating Issues

#### The Suicidal Kavu Problem

<div class="row">
    <div class="col-sm-8">
        <p>Some Magic Cards will force the player to hurt themselves or their own creatures because of how the cards are templated. For example, the way the classic card Flametongue Kavu is templated, if you play it on an empty board, you are forced to kill itself with its own ability. The fact that this is going to happen is not immediately obvious to most players, and leads to some terrible feel bads. This can happen with many different triggered effects that the player can’t precisely control.</p>
        <p>When you are designing a card, make sure to not to let this problem happen to you. The easiest way to prevent these kinds of situations is to add "may" (so a player can choose to not let the damage go through) or restrict the targeting to the only things “an opponent controls”. Though this does remove the flexibility of killing your own creatures, that is a niche scenario, and the “opponent controls” restriction still allows the player to hit what they want to 99% of the time.</p>
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/flametongue-kavu.png">
    </div>
</div>


#### The Flaky Toughness Boost Problem

<div class="row">
    <div class="col-sm-8">
        <p>Temporary toughness boosts ending before "end of turn" can result in unintuitive deaths because of “state based actions”. The way death by damage works, is that as a turn goes along, the game is constantly checking to see if the amount of damage on a creature is greater than that creature’s toughness. If it is, the creature will be destroyed by that damage. Most of the time this happens because the damage on the creature is increased. However, it can also happen because of the creature’s toughness     decreasing.</p>
        <p>Take a look to the right at the custom card Brave Knight. When a player has this creature in play, they will determine that since it will have 5 toughness during combat, it will survive being blocked by a 4 power creature. However, once combat ends during their turn, the knight will no longer be attacking, and will lose its toughness boost. This means it will actually die to taking even just 2 damage during combat. This toughness boost is completely useless, and will lead players to making incorrect decisions.</p>
        <p>Avoid this by making the same ability triggered instead, with the toughness boost wearing off at end of turn. You can see this in the fixed version. During the cleanup step, the toughness boost will go away, but so will the damage marked on the creature. It will now be able to survive the situations the players already thought it could.</p>
        <p>Alternatively, you can make it get the bonus "during your turn."</p>
    </div>
    <div class="col-sm-4">
       <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/brave-knight.png">
       <br>
       <br>
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/brave-knight-fixed.png">
    </div>
</div>

#### The Layers Problem

<div class="row">
    <div class="col-sm-8">
        <p>The way the Magic rules calculate certain things can be unintuitive. Especially stacking effects or effects that are changed by other effects can get very complicated These are worked out in a rules system called <a href="https://magic.wizards.com/en/articles/archive/layer-system-2009-11-05">layers</a>) You can see a condensed graphic describing layers <a href="https://cdn.discordapp.com/attachments/205457071380889601/226507979619434496/IMG_1744.PNG">here</a> and the comprehensive rules for layers <a href="https://mtg.gamepedia.com/Interaction_of_continuous_effects">here</a>).</p>
        <p>The order of these layers is important, because it determines which static (continuous) effects can actually combine properly. You don’t need to memorize them, but realize that some designs will not work intuitively because of the order of layers.</p>
        <p>To the right is an example of a card that works strangely because of layers. A 3/3 creature you control would correctly gain lifelink from this card.  However, a 2/2 creature with a +1/+1 counter on it would, unintuitively, *not *gain lifelink from this card. That is because the layers system gives out keywords before it calculates power/toughness changes due to counters, auras, etc.</p>
        <p>Switching this to grant the lifelink on a trigger solves this problem, since layers will no longer be relevant. Look out for issues caused by layers with your designs that have continuous effects on the board.</p>
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/blessing-of-layers.png">
        <br>
        <br>
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/blessing-of-layers-fixed.png">
    </div>
</div>

#### The Disloyal Planeswalker Problem

<div class="row">
    <div class="col-sm-8">
        <p>Planeswalkers are fun to design, and creating abilities for them is usually pretty intuitive. However, designing plus loyalty abilities (+1, +2, etc.) can be trickier than it seems. The player will almost always want to be able to use their planeswalker’s plus loyalty abilities, even if they can’t get any use out of the ability’s effect. For example, if a planeswalker has the ability "+1: This deals 1 damage to target creature.", the player will often want to use it even if there aren’t any creatures to deal damage to.</p>
        <p> However, the way targeting works, the player can’t activate this ability unless there is a valid target. This means they can’t increase the loyalty the way they want to. Use “up to” to alleviate this, so the player can choose zero targets: “+1: This deals 1 damage to up to one target creature.”</p>
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/evil-fire-wizard-of-bad-plusones.png">
        <br>
        <br>
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/evil-fire-wizard-of-good-plusones.png">
    </div>
</div>