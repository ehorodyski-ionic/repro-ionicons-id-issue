# Ionicons: ID Naming Issue

Particular group IDs prevent icons from rendering.

## Example

Within `src/assets/ic_assignment_ind.svg`, there is a group ID named `One-Page-App--states-pop-up-Applications`. This causes the following markup to be rendered within the Shadow DOM:

```
<div class="icon-inner"></div>
```

However, if you modify `One-Page-App--states-pop-up-Applications` to `ne-Page-App--states-pop-up-Applications` the following is rendered:

```
<div class="icon-inner"><svg viewBox="0 0 18 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="s-ion-icon">
    <!-- Generator: Sketch 59.1 (86144) - https://sketch.com -->
    <title>Icon/ic_assignment_ind</title>
    <desc>Created with Sketch.</desc>
    <g id="ne-Page-App--states-pop-up-Applications" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
        <g id="ICONS_Info-Copy" transform="translate(-102.000000, -478.000000)">
            <g id="Icon/ic_assignment_ind" transform="translate(99.000000, 477.000000)">
                <g id="Icon-24px">
                    <g>
                        <polygon id="Shape" points="0 0 24 0 24 24 0 24"></polygon>
                        <path d="M19,3 L14.82,3 C14.4,1.84 13.3,1 12,1 C10.7,1 9.6,1.84 9.18,3 L5,3 C3.9,3 3,3.9 3,5 L3,19 C3,20.1 3.9,21 5,21 L19,21 C20.1,21 21,20.1 21,19 L21,5 C21,3.9 20.1,3 19,3 L19,3 Z M12,3 C12.55,3 13,3.45 13,4 C13,4.55 12.55,5 12,5 C11.45,5 11,4.55 11,4 C11,3.45 11.45,3 12,3 L12,3 Z M12,7 C13.66,7 15,8.34 15,10 C15,11.66 13.66,13 12,13 C10.34,13 9,11.66 9,10 C9,8.34 10.34,7 12,7 L12,7 Z M18,19 L6,19 L6,17.6 C6,15.6 10,14.5 12,14.5 C14,14.5 18,15.6 18,17.6 L18,19 L18,19 Z" id="Shape" fill="#000000"></path>
                    </g>
                </g>
            </g>
        </g>
    </g>
</svg></div>
```
