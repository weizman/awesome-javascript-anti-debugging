function hashCode (s) {
    var hash = 0;
    if (s.length == 0) {
        return hash;
    }
    for (var i = 0; i < s.length; i++) {
        var char = s.charCodeAt(i);
        hash = ((hash<<5)-hash)+char;
        hash = hash & hash; // Convert to 32bit integer
    }
    return hash;
}

function start() {
    alert('steal cookies!');
}

function main() {
    if (hashCode(start.toString()) !== -1968638942) return;
    start();
}

main()
