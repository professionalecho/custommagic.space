---
layout: default
title: Wording Tips
---
<div class="row">
    <div class="col-sm-12">
        <h3>The Golden Rule</h3>
        <p><b>Always</b> check existing Magic cards to find correct wording. Get good at using <a href="http://www.scryfall.com">Scryfall</a>'s rules text search function to find the snippet that you think you need, to see if it's been printed before. For example, typing <a href="https://scryfall.com/search?q=o%3A%22becomes+snow%22">o:"becomes snow"</a> gives you every instance of a card saying the phrase "becomes snow" in its rules text. There's only two, but the fact that there is precedent means that you can safely use the wording for your own effect.</p>
        <p>It isn't enough to see that cards have the wording you want, though - you should check the rules text in context, to be certain that it's using it the way you want. Precision is key.</p>
    </div>
</div>
<div class="row">
    <div class="col-sm-12">
        <h3>Triggered Abilities vs. Replacement Effects</h3>
    </div>
</div>
<div class="row">
    <div class="col-sm-6">
        <p>A <b>triggered ability</b> begins with the word "when", "whenever", or "at". It indicates that the ability happens after the trigger condition (e.g. Thornbow Archer has to be declared as an attacker order for its ability to trigger).</p>
    </div>
    <div class="col-sm-6">
        <p>A <b>replacement effect</b> begins with the word "if", and uses the word "instead". It indicates that the effect that would have occurred does not occur, and the replacement effect occurs instead.</p>
    </div>
</div>
<div class="row">
    <div class="col-sm-6">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/thornbow-archer.png">
        <p>Triggered abilities beginning with "whenever" indicate that the ability might trigger multiple times from that object. Triggered abilities beginning with "when" indicate that the ability is expected to only trigger once (such as an enter-the-battlefield effect).</p>
    </div>
    <div class="col-sm-6">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/fiery-impulse.png">
        <p>More obscure replacement effects include regeneration and "This creature enters the battlefield with..." effects such as <a href="https://scryfall.com/card/cns/67">Apex Hawks</a> or <a href="https://scryfall.com/card/zen/13">Iona, Shield of Emeria</a>.</p>
    </div>
</div>
<div class="row">
    <div class="col-sm-12">
        <h3>Activated Abilities and Costs</h3>
    </div>
</div>
<div class="row">
    <div class="col-sm-6">
        <p>An activated ability can be identified by a colon separating the <b>cost</b> and <b>effect</b>.</p>
        <p>Akroan Jailer's activated ability has a cost made up of two parts. The first requires mana - <i class="ms ms-cost ms-2"></i><i class="ms ms-cost ms-w"></i> - and the second requires the creature to tap - <i class="ms ms-cost ms-tap"></i>. These parts to the cost are separated by a comma.</p>
        <p>Costs can theoretically be made up of anything, including discarding cards, paying life, or revealing a card from your hand. There are some very strange costs including "Draw a card" on <a href="https://scryfall.com/card/wth/50">Psychic Vortex</a> or "Add <i class="ms ms-cost ms-r"></i> to your mana pool" on <a href="https://scryfall.com/card/csp/78">Braid of Fire</a>, but as a general rule try to keep your costs to things that require expending resources. Everything else should be part of the effect.</p>

    </div>
    <div class="col-sm-6">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/akroan-jailer.png">
    </div>
</div>
<div class="row">
    <div class="col-sm-12">
        <h3>Permanents, Spells, and Cards</h3>
    </div>
</div>
<div class="row">
    <div class="col-sm-4">
        <p>A card references a <b>creature</b> when it wants to affect one currently on the battlefield.</p>
    </div>
    <div class="col-sm-4">
        <p>A card references a <b>creature spell</b> when it wants to affect one on the stack.</p>
    </div>
    <div class="col-sm-4">
        <p>A card references a <b>creature card</b> when it wants to affect one in a graveyard, in exile, in a hand, or in a library.</p>
    </div>
</div>
<div class="row">
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/doom-blade.png">
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/exclude.png">
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/macabre-waltz.png">
    </div>
</div>
<div class="row">
    <div class="col-sm-12">
       <br>
        <p>This rule is true of <b>all card types</b>.</p>
    </div>
</div>
<div class="row">
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/acidic-slime.png">
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/dispel.png">
    </div>
    <div class="col-sm-4">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/call-the-gatewatch.png">
    </div>
</div>
<br>
<div class="row">
    <div class="col-sm-12">
        <h3>Damage Sources</h3>
    </div>
</div>
<div class="row">
    <div class="col-sm-6">
        <p>Damage <i>always</i> requires a source and a recipient. The source is generally the card dealing the damage, though not in every case.</p>
        <p><b>CORRECT:</b> Flame Slash deals 4 damage to target creature..</p>
        <p><b>INCORRECT:</b> Target creature takes 4 damage.</p>
        <p><b>INCORRECT:</b> Deal 4 damage to target creature.</p>
        <p>If the effect involves the controller being dealt damage, consider using "Pay N life" instead, such as on <a href="https://scryfall.com/card/jou/163">Mana Confluence</a>.</p>
        <p>On the majority of black cards, players "lose life" instead, such as on <a href="https://scryfall.com/card/m10/83">Acolyte of Xathrid</a>. This does not count as damage for the purposes of prevention such as <a href="https://scryfall.com/card/dis/1">Aurora Eidolon</a>.</p>
    </div>
    <div class="col-sm-6">
        <img class="img-fluid" src="{{ site.baseurl }}/css/imgs/flame-slash.png">
    </div>
</div>
<div class="row">
    <div class="col-sm-12">
        <h3>More Wording</h3>
    </div>
    <div class="col-sm-6">
        <p>The <a href="https://www.reddit.com/r/custommagic/wiki/index#wiki_.2Fr.2Fcustommagic_custom_renders">/r/custommagic wiki</a> has plenty more tips on how to word things. Also, see the table for more MSE shortcuts. The CARDNAME and LEGENDNAME shortcuts are invaluable for keeping your card name consistent through the text. Failing that, never forget the golden rule!</p>
    </div>
    <div class="col-sm-6">
        <table class="table table-responsive">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Shortcut</th>
                    <th>Result</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Name of card</td>
                    <td>~</td>
                    <td>CARDNAME</td>
                </tr>
                <tr>
                    <td>Short name of card</td>
                    <td>@</td>
                    <td>LEGENDNAME</td>
                </tr>
                <tr>
                    <td>Bullet point</td>
                    <td>::</td>
                    <td>&bull;</td>
                </tr>
                <tr>
                    <td>Em Dash</td>
                    <td>--</td>
                    <td>&mdash;</td>
                </tr>
            </tbody>  
    </table>
</div>
</div>