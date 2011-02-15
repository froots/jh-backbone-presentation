# Controllers

## Example Route

<pre class="brush: js">
    index: function() {
        var channelsCollection = new ChannelsCollection();
        var channelsView = new ChannelsView({
            collection: channelsCollection
        });
        channelsCollection.fetch();
    }
</pre>

* fetch loads and parses channel data from server
* channelsView subscribes to collection 'refresh' event
* channelsView renders data from collection