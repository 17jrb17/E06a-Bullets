# E06a-Bullets
I'm gonna be honest I finished this in class while you were showing me how to do it and then just forgot to push it so my apologies. Basically what I did is generate a bullet and with your help figured out how to detect when each current bullet collides with an enemy sprite and when it does it kills the bullet while damaging the enemy and increasing score until all the enemy sprites are killed. Again, sorry this is late, if I get a 0 I understand I goofed up.

For extra credit, end the game when all the penguins have been killed.

I will award significant extra credit if you subsequently create a main2.py, using the same framework, that allows the penguins to fire back. I have included a bullet_enemy.png asset for that purpose. Even more points will be awarded if you include explosions and/or damage indicators.

To get you started, this is how I generated a new bullet:

```
    x = self.player.center_x
    y = self.player.center_y + 15
    bullet = Bullet((x,y),(0,10),BULLET_DAMAGE)
    self.bullet_list.append(bullet)
```

The arcade.check_for_collision_with_list(sprite, spriteList) method takes a sprite and a spriteList and returns a list of any elements from spriteList that are currently colliding with sprite.

self.player.kill() will remove the player sprite. .kill() can be (similarly) used to remove any sprite.

As always, let me know if you have any questions.