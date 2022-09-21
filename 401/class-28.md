# Recycler View

Used to display data on screen as it's visibly available. If it's not the element is recycled and the resourses are given to another element. Vastly improving performance.

### Key Classes
 - Recycler view is a viewgroup that can be added to the Ui like any other viewgroup.
 - Each element is defined by a view holder object. you define the viewholder by extending recyclerview.viewholder.
 - Recyclerview requests the views and binds them to their data.

### Steps for implementing
 - First of all, decide what the list or grid is going to look like. Ordinarily you'll be able to use one of the RecyclerView library's standard layout managers.  
 - Design how each element in the list is going to look and behave.
 - Define the Adapter that associates your data with the ViewHolder views.
 - [advanced customization](https://developer.android.com/develop/ui/views/layout/recyclerview-custom)

### Layout
A layout manager class handles the three most common layouts.
 - LinearLayoutManager arranges the items in a one-dimensional list.
 - GridLayoutManager arranges all items in a two-dimensional grid.
    - If the grid is arranged vertically, GridLayoutManager tries to make all the elements in each row have the same width and height, but different rows can have different heights.
    - If the grid is arranged horizontally, GridLayoutManager tries to make all the elements in each column have the same width and height, but different columns can have different widths.
 - StaggeredGridLayoutManager is similar to GridLayoutManager, but it does not require that items in a row have the same height (for vertical grids) or items in the same column have the same width (for horizontal grids). The result is that the items in a row or column can end up offset from each other.
 
### Example

````
public class CustomAdapter extends RecyclerView.Adapter<CustomAdapter.ViewHolder> {

    private String[] localDataSet;

    /**
     * Provide a reference to the type of views that you are using
     * (custom ViewHolder).
     */
    public static class ViewHolder extends RecyclerView.ViewHolder {
        private final TextView textView;

        public ViewHolder(View view) {
            super(view);
            // Define click listener for the ViewHolder's View

            textView = (TextView) view.findViewById(R.id.textView);
        }

        public TextView getTextView() {
            return textView;
        }
    }

    /**
     * Initialize the dataset of the Adapter.
     *
     * @param dataSet String[] containing the data to populate views to be used
     * by RecyclerView.
     */
    public CustomAdapter(String[] dataSet) {
        localDataSet = dataSet;
    }

    // Create new views (invoked by the layout manager)
    @Override
    public ViewHolder onCreateViewHolder(ViewGroup viewGroup, int viewType) {
        // Create a new view, which defines the UI of the list item
        View view = LayoutInflater.from(viewGroup.getContext())
                .inflate(R.layout.text_row_item, viewGroup, false);

        return new ViewHolder(view);
    }

    // Replace the contents of a view (invoked by the layout manager)
    @Override
    public void onBindViewHolder(ViewHolder viewHolder, final int position) {

        // Get element from your dataset at this position and replace the
        // contents of the view with that element
        viewHolder.getTextView().setText(localDataSet[position]);
    }

    // Return the size of your dataset (invoked by the layout manager)
    @Override
    public int getItemCount() {
        return localDataSet.length;
    }
}
````

#### resources used
[android recycler view docs](https://developer.android.com/develop/ui/views/layout/recyclerview#java)
