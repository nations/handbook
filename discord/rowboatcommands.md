<div class="page-inner">
                            
<div id="book-search-results">
    <div class="search-noresults">
    
                                <section class="normal markdown-section">
                                
                                <h1 id="moderator-command-quick-reference">Moderator Command Quick-Reference</h1>
<h2 id="punishments">Punishments</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>warn {user} [reason]</code></td>
<td>Adds a warning infraction to a user</td>
<td>Moderator</td>
<td><code>>warn 232921983317180416 1st warning, spamming emoji</code> OR <code>>warn @rowboat#0001 2nd warning, going off-topic</code></td>
</tr>
<tr>
<td><code>>mute {user} [reason]</code></td>
<td>Mutes a user. This will only work if <code>mute_role</code> is set in the config</td>
<td>Moderator</td>
<td><code>>mute 232921983317180416 spamming</code> OR  <code>>tempmute @rowboat#0001 60m spamming</code></td>
</tr>
<tr>
<td><code>>unmute {user}</code></td>
<td>Unmutes a user</td>
<td>Moderator</td>
<td><code>>unmute 232921983317180416</code></td>
</tr>
<tr>
<td><code>>tempmute {user} {duration} [reason]</code></td>
<td>Temporarily mutes a user. Will only work if <code>temp_mute_role</code> or <code>mute_role</code> is set in the config</td>
<td>Moderator</td>
<td><code>>tempmute 232921983317180416 30m spamming</code> OR <code>>tempmute @rowboat#0001 30m spamming</code></td>
</tr>
<tr>
<td><code>>kick {user} [reason]</code></td>
<td>Kicks the user from the server</td>
<td>Moderator</td>
<td><code>>kick 232921983317180416 spamming</code> OR <code>>kick @rowboat#0001 spamming</code></td>
</tr>
<tr>
<td><code>>ban {user} [reason]</code></td>
<td>Bans a user from the server</td>
<td>Moderator</td>
<td><code>>ban 232921983317180416 spamming</code> OR <code>>ban @rowboat#0001 spamming</code></td>
</tr>
<tr>
<td><code>>unban {user} [reason]</code></td>
<td>Unbans a user</td>
<td>Moderator</td>
<td><code>>unban 232921983317180416</code></td>
</tr>
<tr>
<td><code>>forceban {User ID} [reason]</code></td>
<td>Force bans a user who is not currently in the server</td>
<td>Moderator</td>
<td><code>>forceban 232921983317180416 spamming</code></td>
</tr>
<tr>
<td><code>>softban {user} [reason]</code></td>
<td>Softbans (bans/unbans) a user and deletes the user's messages sent within the last 7 days</td>
<td>Moderator</td>
<td><code>>softban 232921983317180416 spamming</code> OR <code>>softban @rowboat#0001 spamming</code></td>
</tr>
<tr>
<td><code>>tempban {user} {duration} [reason]</code></td>
<td>Temporarily bans a user</td>
<td>Moderator</td>
<td><code>>tempban 232921983317180416 5h spamming</code> OR <code>>tempban @rowboat#0001 5h spamming</code></td>
</tr>
</tbody>
</table>
<h2 id="admin-utilities">Admin Utilities</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>clean all [count]</code></td>
<td>Cleans (deletes) [count] many messages in the current channel</td>
<td>Moderator</td>
<td><code>>clean all 20</code></td>
</tr>
<tr>
<td><code>>clean user {user} [count]</code></td>
<td>Cleans [count] many messages a given user sent in the current channel</td>
<td>Moderator</td>
<td><code>>clean user 232921983317180416 50</code></td>
</tr>
<tr>
<td><code>>clean bots [count]</code></td>
<td>Cleans [count] many messages sent by bots in the current channel</td>
<td>Moderator</td>
<td><code>>clean bots 30</code></td>
</tr>
<tr>
<td><code>>clean cancel</code></td>
<td>Cancels any cleaning process running in current channel</td>
<td>Moderator</td>
<td><code>>clean cancel</code></td>
</tr>
<tr>
<td><code>>reactions clean {user} [count] [emoji]</code></td>
<td>Removes the most recent count of reactions from a given user</td>
<td>Moderator</td>
<td><code>>reactions clean 232921983317180416</code> OR <code>>reactions clean @rowboat#0001 30</code> OR <code>>reactions clean 232921983317180416 20 :thinking:</code></td>
</tr>
<tr>
<td><code>>archive (here / all) [count]</code></td>
<td>Archives [count] many messages in the current channel</td>
<td>Moderator</td>
<td><code>>archive all 50</code> OR <code>>archive here 50</code></td>
</tr>
<tr>
<td><code>>archive user {user} [count]</code></td>
<td>Archives [count] many messages that a given user sent in the current guild</td>
<td>Moderator</td>
<td><code>>archive user 232921983317180416 100</code> OR <code>>archive user @rowboat#0001 100</code></td>
</tr>
<tr>
<td><code>>archive channel {channel} [count]</code></td>
<td>Archives [count] many messages in the given channel</td>
<td>Moderator</td>
<td><code>>archive channel 289482554250100736 20</code></td>
</tr>
<tr>
<td><code>>search {query}</code></td>
<td>Searches for usernames that match given query</td>
<td>Default</td>
<td><code>>search b1nzy</code></td>
</tr>
<tr>
<td><code>>role add {user} {role} [reason]</code></td>
<td>Adds a role to a user</td>
<td>Moderator</td>
<td><code>>role add 232921983317180416 Moderator Promotion from Member</code> OR <code>>role add rowboat#0001 Admin Pretty good Moderator</code></td>
</tr>
<tr>
<td><code>>role remove {user} {role} [reason]</code></td>
<td>Removes a role from a user</td>
<td>Moderator</td>
<td><code>>role remove 232921983317180416 Administrator Demoted for being bad at job</code> OR <code>>role remove rowboat#0001 Mod Terrible moderator</code></td>
</tr>
<tr>
<td><code>>r add {duration} {content}</code> OR <code>>remind {duration} {content}</code></td>
<td>Adds a reminder. Bot will mention the user after the specified duration with the given message</td>
<td>Default</td>
<td><code>>r add 24h update announcements</code> OR <code>>remind 24h update announcements</code></td>
</tr>
<tr>
<td><code>>r clear</code></td>
<td>Clears all of the user's reminders</td>
<td>Default</td>
<td><code>>r clear</code></td>
</tr>
<tr>
<td><code>>voice log {user}</code></td>
<td>Displays a list of a given user's recent voice channel activity</td>
<td>Moderator</td>
<td><code>>voice log 232921983317180416</code> OR <code>>voice log @rowboat#0001</code></td>
</tr>
</tbody>
</table>
<h2 id="infractions">Infractions</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>infractions search {query}</code></td>
<td>Searches infractions database for given query</td>
<td>Moderator</td>
<td><code>>infractions search 232921983317180416</code> OR <code>>infractions search rowboat#0001</code> OR <code>>infractions search spamming</code></td>
</tr>
<tr>
<td><code>>infractions info {inf#}</code></td>
<td>Presents information on the given infraction</td>
<td>Moderator</td>
<td><code>>infractions info 1274</code></td>
</tr>
<tr>
<td><code>>infractions duration {inf#} {duration}</code></td>
<td>Updates the duration of the given infraction. Duration starts from time of initial action</td>
<td>Moderator</td>
<td><code>>infractions duration 1274 5h</code></td>
</tr>
<tr>
<td><code>>reason {inf#} {reason}</code></td>
<td>Updates the reason of a given infraction</td>
<td>Moderator</td>
<td><code>>reason 1274 rude behaviour towards staff</code></td>
</tr>
</tbody>
</table>
<h2 id="starboard">Starboard</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>stars block {user}</code></td>
<td>Prevents the user from starring any messages and prevents their messages from being starred</td>
<td>Moderator</td>
<td><code>>stars block @rowboat#0001</code> OR <code>>stars block 232921983317180416</code></td>
</tr>
<tr>
<td><code>>stars unblock {user}</code></td>
<td>Unblocks a user from the starboard</td>
<td>Moderator</td>
<td><code>>stars unblock @rowboat#0001</code> OR <code>>stars unblock 232921983317180416</code></td>
</tr>
<tr>
<td><code>>stars hide {mid}</code></td>
<td>Hides a starred message from the starboard</td>
<td>Moderator</td>
<td><code>>stars hide 320312743842545664</code></td>
</tr>
<tr>
<td><code>>stars unhide {mid}</code></td>
<td>Unhides a hidden message</td>
<td>Moderator</td>
<td><code>>stars unhide 320312743842545664</code></td>
</tr>
<tr>
<td><code>>stars lock</code></td>
<td>Prevents any new starred messages from being posted to the starboard</td>
<td>Administrator</td>
<td><code>>stars lock</code></td>
</tr>
<tr>
<td><code>>stars unlock</code></td>
<td>Enables starred messages to be posted</td>
<td>Administrator</td>
<td><code>>stars unlock</code></td>
</tr>
</tbody>
</table>

                                
                                </section>
                            
    </div>            
        </div>
    </div>
</div>

<div class="page-inner">
                            
<div id="book-search-results">
    <div class="search-noresults">
    
                                <section class="normal markdown-section">
                                
                                <h1 id="utility-plugin">Utility Plugin</h1>
<p>The utility plugin provides a number of useful and fun commands</p>
<h2 id="commands">Commands</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>cat</code></td>
<td>Returns a random image of a cat</td>
<td>Default</td>
<td><code>>cat</code></td>
</tr>
<tr>
<td><code>>emoji {emoji}</code></td>
<td>Returns information on the given emoji</td>
<td>Default</td>
<td><code>>emoji :smiley:</code></td>
</tr>
<tr>
<td><code>>info {user}</code></td>
<td>Returns information on the given user</td>
<td>Default</td>
<td><code>>info 232921983317180416</code> OR <code>>info @rowboat#0001</code></td>
</tr>
<tr>
<td><code>>jumbo {emojis}</code></td>
<td>Returns 128x128px images of the given emoji</td>
<td>Default</td>
<td><code>>jumbo :cat: :dog: :rabbit:</code></td>
</tr>
<tr>
<td><code>>random coin</code></td>
<td>Flips a coin and returns the result</td>
<td>Default</td>
<td><code>>random coin</code></td>
</tr>
<tr>
<td><code>>random number [end number] [start number]</code></td>
<td>Returns a random number from 0-10 or in a range if specified</td>
<td>Default</td>
<td><code>>random number</code> OR <code>>random number 50 20</code></td>
</tr>
<tr>
<td><code>>r add {duration} {content}</code> OR <code>>remind {duration} {content}</code></td>
<td>Adds a reminder. Bot will mention the user after the specified duration with the given message</td>
<td>Default</td>
<td><code>>r add 24h update announcements</code> OR <code>>remind 24h update announcements</code></td>
</tr>
<tr>
<td><code>>r clear</code></td>
<td>Clears all of the user's reminders</td>
<td>Default</td>
<td><code>>r clear</code></td>
</tr>
<tr>
<td><code>>search {query}</code></td>
<td>Searches for usernames that match given query</td>
<td>Default</td>
<td><code>>search b1nzy</code></td>
</tr>
<tr>
<td><code>>seen {user}</code></td>
<td>Returns the timestamp of when the bot last saw a message from given user</td>
<td>Default</td>
<td><code>>seen 232921983317180416</code> OR <code>>seen @rowboat#0001</code></td>
</tr>
<tr>
<td><code>>server [guild]</code></td>
<td>Returns information on the current server or the Server ID if given</td>
<td>Default</td>
<td><code>>server</code> OR <code>>server 290923757399310337</code></td>
</tr>
</tbody>
</table>
<h2 id="configuration-example">Configuration Example</h2>
<pre><code>utilities: {}
</code></pre><p>There is no further configuration for this plugin.</p>

                                
                                </section>
                            
    </div>
        </div>
    </div>
</div>

<div class="page-inner">
                            
<div id="book-search-results">
    <div class="search-noresults">
    
                                <section class="normal markdown-section">
                                
                                <h1 id="admin-plugin">Admin Plugin</h1>
<p>The admin plugin provides a set of administrator commands that help in moderating active servers.</p>
<h2 id="commands">Commands</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>join / add / give {role}</code></td>
<td>Assigns a role if it's listed in the group_roles config setting</td>
<td>Default</td>
<td><code>>join PC</code> OR <code>>add Console</code> OR <code>>give Tabletop</code></td>
</tr>
<tr>
<td><code>>leave / remove / take {role}</code></td>
<td>Removes a group role from a user</td>
<td>Default</td>
<td><code>>leave PC</code> OR <code>>remove Console</code> OR <code>>take Tabletop</code></td>
</tr>
<tr>
<td><code>>temprole {user} {role ID} {duration} [reason]</code></td>
<td>Temporarily applies a role to a user</td>
<td>Moderator</td>
<td><code>>temprole 232921983317180416 295646805650046977 7d Trial Mod</code> OR <code>>temprole @rowboat#0001 295646805650046977 24h Member of the Day</code></td>
</tr>
<tr>
<td><code>>roles</code></td>
<td>Returns a list of ids/names for all roles on the server. Useful for configuring other rowboat plugins</td>
<td>Moderator</td>
<td><code>>roles</code></td>
</tr>
<tr>
<td><code>>role add {user} {role} [reason]</code></td>
<td>Adds a role to a user</td>
<td>Moderator</td>
<td><code>>role add 232921983317180416 Moderator Promotion from Member</code> OR <code>>role add rowboat#0001 Admin Pretty good Moderator</code></td>
</tr>
<tr>
<td><code>>role remove {user} {role} [reason]</code></td>
<td>Removes a role from a user</td>
<td>Moderator</td>
<td><code>>role remove 232921983317180416 Administrator Demoted for being bad at job</code> OR <code>>role remove rowboat#0001 Mod Terrible moderator</code></td>
</tr>
<tr>
<td><code>>role unlock {role ID}</code></td>
<td>Unlocks a role listed in the locked_roles config setting for 5 minutes, allowing permission updates</td>
<td>Administrator</td>
<td><code>>role unlock 346471724126044160</code></td>
</tr>
<tr>
<td><code>>archive (here / all) [count]</code></td>
<td>Archives [count] many messages in the current channel</td>
<td>Moderator</td>
<td><code>>archive all 50</code> OR <code>>archive here 50</code></td>
</tr>
<tr>
<td><code>>archive user {user} [count]</code></td>
<td>Archives [count] many messages that a given user sent in the current guild</td>
<td>Moderator</td>
<td><code>>archive user 232921983317180416 100</code> OR <code>>archive user @rowboat#0001 100</code></td>
</tr>
<tr>
<td><code>>archive channel {channel} [count]</code></td>
<td>Archives [count] many messages in the given channel</td>
<td>Moderator</td>
<td><code>>archive channel 289482554250100736 20</code></td>
</tr>
<tr>
<td><code>>clean all [count]</code></td>
<td>Cleans (deletes) [count] many messages in the current channel</td>
<td>Moderator</td>
<td><code>>clean all 20</code></td>
</tr>
<tr>
<td><code>>clean user {user} [count]</code></td>
<td>Cleans [count] many messages a given user sent in the current channel</td>
<td>Moderator</td>
<td><code>>clean user 232921983317180416 50</code></td>
</tr>
<tr>
<td><code>>clean bots [count]</code></td>
<td>Cleans [count] many messages sent by bots in the current channel</td>
<td>Moderator</td>
<td><code>>clean bots 30</code></td>
</tr>
<tr>
<td><code>>clean cancel</code></td>
<td>Cancels any cleaning process running in current channel</td>
<td>Moderator</td>
<td><code>>clean cancel</code></td>
</tr>
<tr>
<td><code>>reactions clean {user} [count] [emoji]</code></td>
<td>Removes the most recent count of reactions from a given user</td>
<td>Moderator</td>
<td><code>>reactions clean 232921983317180416</code> OR <code>>reactions clean @rowboat#0001 30</code> OR <code>>reactions clean 232921983317180416 20 :thinking:</code></td>
</tr>
<tr>
<td><code>>backups restore {user}</code></td>
<td>Restores a user to the most recently saved member backup</td>
<td>Moderator</td>
<td><code>>backups restore 232921983317180416</code> OR <code>>backups restore rowboat#0001</code></td>
</tr>
<tr>
<td><code>>backups clear {user ID}</code></td>
<td>Deletes all saved backups for a user</td>
<td>Moderator</td>
<td><code>>backups clear 232921983317180416</code> OR <code>>backups clear rowboat#0001</code></td>
</tr>
<tr>
<td><code>>stats {user}</code></td>
<td>Presents general statistics for a given user</td>
<td>Moderator</td>
<td><code>>stats 232921983317180416</code> OR <code>>stats rowboat#0001</code></td>
</tr>
<tr>
<td><code>>emojistats (global / server) most</code></td>
<td>Displays the most / least used server emojis in the current guild / globally</td>
<td>Moderator</td>
<td><code>>emojistats global most</code> OR <code>>emojistats server least</code></td>
</tr>
<tr>
<td><code>>voice log {user}</code></td>
<td>Displays a list of a given user's recent voice channel activity</td>
<td>Moderator</td>
<td><code>>voice log 232921983317180416</code> OR <code>>voice log @rowboat#0001</code></td>
</tr>
<tr>
<td><code>>invites prune [uses]</code></td>
<td>Deletes server invites with the given number of uses or less. Cleans 1 and 0 use invites if left blank</td>
<td>Administrator</td>
<td><code>>invites prune 5</code></td>
</tr>
</tbody>
</table>
<h2 id="configuration-options">Configuration Options</h2>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>role_aliases</td>
<td>Aliases which can be used in place of role IDs in commands</td>
<td>dict</td>
<td>empty</td>
</tr>
<tr>
<td>group_roles</td>
<td>Roles which can be joined and left by any user. These roles cannot grant any elevated permissions</td>
<td>dict</td>
<td>empty</td>
</tr>
<tr>
<td>locked_roles</td>
<td>Prevents permission changes from being made to listed roles</td>
<td>list</td>
<td>empty</td>
</tr>
<tr>
<td>persist</td>
<td>Controls the member persistance settings</td>
<td>dict</td>
<td>empty</td>
</tr>
</tbody>
</table>
<h3 id="member-persistance-settings">Member Persistance Settings</h3>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>roles</td>
<td>Whether to recover roles when a user rejoins the server</td>
<td>bool</td>
<td>false</td>
</tr>
<tr>
<td>role_ids</td>
<td>A list of role ids which will be recovered if <code>roles</code> is true. Any other roles will be ignored when a user rejoins the server</td>
<td>list</td>
<td>empty</td>
</tr>
<tr>
<td>nickname</td>
<td>Whether to recover the nickname when a user rejoins the server</td>
<td>bool</td>
<td>false</td>
</tr>
<tr>
<td>voice</td>
<td>Whether to recover mute/deafen settings when a user rejoins the server</td>
<td>bool</td>
<td>false</td>
</tr>
</tbody>
</table>
<h2 id="configuration-example">Configuration Example</h2>
<pre><code>  admin:
    persist:
      roles: true
      role_ids: [278810978722906112, 278972423502561280, 278972377587515392]
      nickname: true
      voice: false
    role_aliases:
      role1: 205769314199011329
      role2: 333806119199703042
    group_roles:
      PC: 278810978722906112
      Console: 278972377587515392
      Tabletop: 278972423502561280
    locked_roles: [346471724126044160, 252184905075654657]
</code></pre>
                                
                                </section>
                            
    </div>
</div>

<div class="page-inner">
                            
<div id="book-search-results">
    <div class="search-noresults">
    
                                <section class="normal markdown-section">
                                
                                <h1 id="infractions-plugin">Infractions Plugin</h1>
<p>The infractions plugin provides a set of useful moderator commands. These commands are intended to be used together and help handle/track misbehaving users over time.</p>
<h2 id="commands">Commands</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>warn {user} [reason]</code></td>
<td>Adds a warning infraction to a user</td>
<td>Moderator</td>
<td><code>>warn 232921983317180416 1st warning, spamming emoji</code> OR <code>>warn @rowboat#0001 2nd warning, going off-topic</code></td>
</tr>
<tr>
<td><code>>mute {user} [reason]</code></td>
<td>Mutes a user. This will only work if <code>mute_role</code> is set in the config</td>
<td>Moderator</td>
<td><code>>mute 232921983317180416 spamming</code> OR  <code>>tempmute @rowboat#0001 60m spamming</code></td>
</tr>
<tr>
<td><code>>unmute {user}</code></td>
<td>Unmutes a user</td>
<td>Moderator</td>
<td><code>>unmute 232921983317180416</code></td>
</tr>
<tr>
<td><code>>tempmute {user} {duration} [reason]</code></td>
<td>Temporarily mutes a user. Will only work if <code>temp_mute_role</code> or <code>mute_role</code> is set in the config</td>
<td>Moderator</td>
<td><code>>tempmute 232921983317180416 30m spamming</code> OR <code>>tempmute @rowboat#0001 30m spamming</code></td>
</tr>
<tr>
<td><code>>kick {user} [reason]</code></td>
<td>Kicks the user from the server</td>
<td>Moderator</td>
<td><code>>kick 232921983317180416 spamming</code> OR <code>>kick @rowboat#0001 spamming</code></td>
</tr>
<tr>
<td><code>>mkick {users] -r [reason]</code></td>
<td>Kicks multiple users from the server</td>
<td>Moderator</td>
<td><code>>mkick 232921983317180416 80351110224678912 108598213681922048 -r spamming</code></td>
</tr>
<tr>
<td><code>>ban {user} [reason]</code></td>
<td>Bans a user from the server</td>
<td>Moderator</td>
<td><code>>ban 232921983317180416 spamming</code> OR <code>>ban @rowboat#0001 spamming</code></td>
</tr>
<tr>
<td><code>>unban {user} [reason]</code></td>
<td>Unbans a user</td>
<td>Moderator</td>
<td><code>>unban 232921983317180416</code></td>
</tr>
<tr>
<td><code>>forceban {User ID} [reason]</code></td>
<td>Force bans a user who is not currently in the server</td>
<td>Moderator</td>
<td><code>>forceban 232921983317180416 spamming</code></td>
</tr>
<tr>
<td><code>>softban {user} [reason]</code></td>
<td>Softbans (bans/unbans) a user and deletes the user's messages sent within the last 7 days</td>
<td>Moderator</td>
<td><code>>softban 232921983317180416 spamming</code> OR <code>>softban @rowboat#0001 spamming</code></td>
</tr>
<tr>
<td><code>>tempban {user} {duration} [reason]</code></td>
<td>Temporarily bans a user</td>
<td>Moderator</td>
<td><code>>tempban 232921983317180416 5h spamming</code> OR <code>>tempban @rowboat#0001 5h spamming</code></td>
</tr>
<tr>
<td><code>>infractions archive</code></td>
<td>Creates a CSV file of all infractions on the server</td>
<td>Administrator</td>
<td><code>>infractions archive</code></td>
</tr>
<tr>
<td><code>>infractions search {query}</code></td>
<td>Searches infractions database for given query</td>
<td>Moderator</td>
<td><code>>infractions search 232921983317180416</code> OR <code>>infractions search rowboat#0001</code> OR <code>>infractions search spamming</code></td>
</tr>
<tr>
<td><code>>infractions info {inf#}</code></td>
<td>Presents information on the given infraction</td>
<td>Moderator</td>
<td><code>>infractions info 1274</code></td>
</tr>
<tr>
<td><code>>infractions duration {inf#} {duration}</code></td>
<td>Updates the duration of the given infraction. Duration starts from time of initial action</td>
<td>Moderator</td>
<td><code>>infractions duration 1274 5h</code></td>
</tr>
<tr>
<td><code>>reason {inf#} {reason}</code></td>
<td>Updates the reason of a given infraction</td>
<td>Moderator</td>
<td><code>>infractions reason 1274 rude behaviour towards staff</code></td>
</tr>
</tbody>
</table>
<h2 id="configuration-options">Configuration Options</h2>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>confirm_actions</td>
<td>Whether to confirm that an action was done in the current channel</td>
<td>bool</td>
<td>true</td>
</tr>
<tr>
<td>confirm_actions_reaction</td>
<td>Whether to confirm actions done in the channel using a checkmark reaction</td>
<td>bool</td>
<td>false</td>
</tr>
<tr>
<td>confirm_actions_expiry</td>
<td>The duration after which to delete the confirmed action message. If zero the message will never be deleted</td>
<td>int</td>
<td>0</td>
</tr>
<tr>
<td>mute_role</td>
<td>Role ID that is set for users who are muted</td>
<td>id</td>
<td>none</td>
</tr>
<tr>
<td>reason_edit_level</td>
<td>Minimum level to allow users to edit other users' infraction reasons</td>
<td>int</td>
<td>100</td>
</tr>
</tbody>
</table>
<h2 id="configuration-example">Configuration Example</h2>
<pre><code>  infractions:
    confirm_actions: false
    mute_role: 289494296703533058
    reason_edit_level: 50
</code></pre>
                                
                                </section>
                            
    </div>
    </div>
</div>

<div class="page-inner">
                            
<div id="book-search-results">
    <div class="search-noresults">
    
                                <section class="normal markdown-section">
                                
                                <h1 id="modlog-plugin">ModLog Plugin</h1>
<p>The modlog plugin provides a mechanisim for logging various events and actions to one or more channels. The intention of the modlog is to provide a private feed of server events that administrators and moderators can use to better monitor and audit users actions. The modlog is extremely configurable, and thus fairly complex.</p>
<h2 id="commands">Commands</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>modlog hush</code></td>
<td>Disables tracking of message deletes in modlog</td>
<td>Administrator</td>
<td><code>>modlog hush</code></td>
</tr>
<tr>
<td><code>>modlog unhush</code></td>
<td>Re-enables tracking of message deletes</td>
<td>Administrator</td>
<td><code>>modlog unhush</code></td>
</tr>
</tbody>
</table>
<h2 id="configuration-options">Configuration Options</h2>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>ignored_users</td>
<td>A list of user ids which are ignored in the modlog. This is useful for ignoring bots that regularly delete or edit their messages</td>
<td>list</td>
<td>empty</td>
</tr>
<tr>
<td>ignored_channels</td>
<td>A list of channel ids which are ignored in the modlog. This is useful for ignoring private or high-activity channels</td>
<td>list</td>
<td>empty</td>
</tr>
<tr>
<td>new_member_threshold</td>
<td>The number of seconds an account is considered new</td>
<td>int</td>
<td>900 (15 minutes)</td>
</tr>
<tr>
<td>channels</td>
<td>Mapping of channel names/ids to ModLog Configurations</td>
<td>dict</td>
<td>empty</td>
</tr>
</tbody>
</table>
<h3 id="modlog-configuration">ModLog Configuration</h3>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>include</td>
<td>List of modlog actions to include. If empty this includes all mod log actions</td>
<td>list</td>
<td>empty</td>
</tr>
<tr>
<td>exclude</td>
<td>List of modlog actions to exclude. If empty this excludes no mod log actions</td>
<td>list</td>
<td>empty</td>
</tr>
<tr>
<td>timestamps</td>
<td>Whether to render timestamps along with loglines</td>
<td>bool</td>
<td>false</td>
</tr>
<tr>
<td>timezone</td>
<td>The timezone that timestamps are rendered in. Supported timezones: (<a href="https://gist.github.com/heyalexej/8bf688fd67d7199be4a1682b3eec7568" target="_blank">https://gist.github.com/heyalexej/8bf688fd67d7199be4a1682b3eec7568</a>)</td>
<td>timezone</td>
<td>US/Eastern</td>
</tr>
</tbody>
</table>
<h2 id="actions">Actions</h2>
<table>
<thead>
<tr>
<th>Action</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>CHANNEL_CREATE</td>
<td>A channel is created</td>
</tr>
<tr>
<td>CHANNEL_DELETE</td>
<td>A channel is deleted</td>
</tr>
<tr>
<td>GUILD_MEMBER_ADD</td>
<td>A member joins</td>
</tr>
<tr>
<td>GUILD_MEMBER_REMOVE</td>
<td>A member leaves (or gets kicked)</td>
</tr>
<tr>
<td>GUILD_ROLE_CREATE</td>
<td>A role is created</td>
</tr>
<tr>
<td>GUILD_ROLE_DELETE</td>
<td>A role is deleted</td>
</tr>
<tr>
<td>GUILD_BAN_ADD</td>
<td>A ban is added</td>
</tr>
<tr>
<td>MEMBER_ROLE_ADD</td>
<td>A role is added to a member</td>
</tr>
<tr>
<td>MEMBER_ROLE_RMV</td>
<td>A role is removed from a member</td>
</tr>
<tr>
<td>MEMBER_TEMP_MUTED</td>
<td>A tempmute is added</td>
</tr>
<tr>
<td>MEMBER_MUTED</td>
<td>A mute is added</td>
</tr>
<tr>
<td>MEMBER_UNMUTED</td>
<td>A mute is removed</td>
</tr>
<tr>
<td>MEMBER_KICK</td>
<td>A member is kicked</td>
</tr>
<tr>
<td>MEMBER_BAN</td>
<td>A ban (with a reason) is added</td>
</tr>
<tr>
<td>MEMBER_SOFTBAN</td>
<td>A softban is added</td>
</tr>
<tr>
<td>MEMBER_TEMPBAN</td>
<td>A tempban is added</td>
</tr>
<tr>
<td>MEMBER_WARNED</td>
<td>A warning is added</td>
</tr>
<tr>
<td>MEMBER_RESTORE</td>
<td>A user rejoined and had their roles/nickname/etc restored</td>
</tr>
<tr>
<td>ADD_NICK</td>
<td>A user adds a nickname</td>
</tr>
<tr>
<td>RMV_NICK</td>
<td>A user removes a nickname</td>
</tr>
<tr>
<td>CHANGE_NICK</td>
<td>A user changes their nickname</td>
</tr>
<tr>
<td>CHANGE_USERNAME</td>
<td>A user changes their username</td>
</tr>
<tr>
<td>MESSAGE_EDIT</td>
<td>A message is edited</td>
</tr>
<tr>
<td>MESSAGE_DELETE</td>
<td>A message is deleted</td>
</tr>
<tr>
<td>MESSAGE_DELETE_BULK</td>
<td>Multiple messages are deleted</td>
</tr>
<tr>
<td>VOICE_CHANNEL_JOIN</td>
<td>A user joins a voice channel</td>
</tr>
<tr>
<td>VOICE_CHANNEL_LEAVE</td>
<td>A user leaves a voice channel</td>
</tr>
<tr>
<td>VOICE_CHANNEL_MOVE</td>
<td>A user moves voice channels</td>
</tr>
<tr>
<td>COMMAND_USED</td>
<td>A user uses a rowboat command</td>
</tr>
<tr>
<td>SPAM_DEBUG</td>
<td>A user triggered spam protection</td>
</tr>
<tr>
<td>CENSORED</td>
<td>A user posted a message that was censored by the bot</td>
</tr>
</tbody>
</table>
<h2 id="configuration-example">Configuration Example</h2>
<pre><code>  modlog:
    channels:
      289494042000228352:
        timestamps: true
        timezone: Etc/GMT-8
        exclude: []
        include: []
    ignored_users: [202217402635780096]
    new_member_threshold: 86400
</code></pre>
                                
                                </section>
                            
    </div>
</div>

<div class="page-inner">
                            
<div id="book-search-results">
    <div class="search-noresults">
    
                                <section class="normal markdown-section">
                                
                                <h1 id="starboard-plugin">Starboard Plugin</h1>
<p>The starboard plugin provides an ongoing board of highlighted messages through community voting.</p>
<h2 id="commands">Commands</h2>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Default Level</th>
<th>Usage</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>>stars show {mid}</code></td>
<td>Displays the given starred message</td>
<td>Trusted</td>
<td><code>>stars show 320312743842545664</code></td>
</tr>
<tr>
<td><code>>stars stats [user]</code></td>
<td>Presents starboard statistics for the whole server or the given user</td>
<td>Moderator</td>
<td><code>>stars stats</code> OR <code>>stars stats 232921983317180416</code></td>
</tr>
<tr>
<td><code>>stars block {user}</code></td>
<td>Prevents the user from starring any messages and prevents their messages from being starred</td>
<td>Moderator</td>
<td><code>>stars block @rowboat#0001</code> OR <code>>stars block 232921983317180416</code></td>
</tr>
<tr>
<td><code>>stars unblock {user}</code></td>
<td>Unblocks a user from the starboard</td>
<td>Moderator</td>
<td><code>>stars unblock @rowboat#0001</code> OR <code>>stars unblock 232921983317180416</code></td>
</tr>
<tr>
<td><code>>stars hide {mid}</code></td>
<td>Hides a starred message from the starboard</td>
<td>Moderator</td>
<td><code>>stars hide 320312743842545664</code></td>
</tr>
<tr>
<td><code>>stars unhide {mid}</code></td>
<td>Unhides a hidden message</td>
<td>Moderator</td>
<td><code>>stars unhide 320312743842545664</code></td>
</tr>
<tr>
<td><code>>stars lock</code></td>
<td>Prevents any new starred messages from being posted to the starboard</td>
<td>Administrator</td>
<td><code>>stars lock</code></td>
</tr>
<tr>
<td><code>>stars unlock</code></td>
<td>Enables starred messages to be posted</td>
<td>Administrator</td>
<td><code>>stars unlock</code></td>
</tr>
<tr>
<td><code>>stars check {mid}</code></td>
<td>Updates star reaction count on given message</td>
<td>Administrator</td>
<td><code>>stars check 320312743842545664</code></td>
</tr>
<tr>
<td><code>>stars update</code></td>
<td>Updates reaction count for the whole starboard</td>
<td>Administrator</td>
<td><code>>stars update</code></td>
</tr>
</tbody>
</table>
<h2 id="configuration-options">Configuration Options</h2>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>channels</td>
<td>A mapping of channels to Starboard Configurations</td>
<td>dict</td>
<td>empty</td>
</tr>
</tbody>
</table>
<h3 id="starboard-configuration">Starboard Configuration</h3>
<table>
<thead>
<tr>
<th>Option</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>channels</td>
<td>Sets which channel starred messages should be posted to</td>
<td>dict</td>
<td>empty</td>
</tr>
<tr>
<td>clear_on_delete</td>
<td>Whether a starboard entry is deleted if the original message is deleted</td>
<td>bool</td>
<td>true</td>
</tr>
<tr>
<td>min_stars</td>
<td>Minimum number of star reactions required before a message is posted to the starboard</td>
<td>int</td>
<td>1</td>
</tr>
<tr>
<td>star_color_max</td>
<td>Sets the "max" star level. Changes shading of rich embed bar color per level and gives the starboard entry a different emoji at max level</td>
<td>int</td>
<td>15</td>
</tr>
<tr>
<td>prevent_self_star</td>
<td>Whether to prevent a user from starring their own message</td>
<td>bool</td>
<td>false</td>
</tr>
</tbody>
</table>
<h2 id="configuration-example">Configuration Example</h2>
<pre><code>  starboard:
    channels:
      301118039326457867:
        clear_on_delete: true
        min_stars: 6
        star_color_max: 15
        prevent_self_star: true
</code></pre>
                                
                                </section>
                            
    </div>
</div>